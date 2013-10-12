function ll(...)
  local cmd = {...}
  for i=1,#cmd do
    print(i,' ',cmd[i])
  end
  print('----------')
  tt(lib.join(cmd))
end

function tt(m) 
 local t=lib.split(m)
  if t[1] ~= nil and #t==1 then   
   shell.run(t[1])
  elseif t[1] ~= nil and #t>=1 then   
   shell.run(t[1],unpack(t,2))
  end
end

local arg={...}
if #arg > 0 then
 ll(arg[1],unpack(arg,2))
end
