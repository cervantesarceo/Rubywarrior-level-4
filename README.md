Rubywarrior-level-4
===================
 class Player
 
 def play_turn(warrior)

    if warrior.feel.empty? 
      if warrior.health <15
        if warrior.health<@health
          warrior.walk!
        else
          warrior.rest!
        end
      else
        warrior.walk!
      end
    else
      warrior.attack!
    end
  @health = warrior.health
 end
end
