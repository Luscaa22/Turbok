local v0=string.char;local v1=string.byte;local v2=string.sub;local v3=bit32 or bit ;local v4=v3.bxor;local v5=table.concat;local v6=table.insert;local function v7(v24,v25) local v26={};for v41=1, #v24 do v6(v26,v0(v4(v1(v2(v24,v41,v41 + 1 )),v1(v2(v25,1 + (v41% #v25) ,1 + (v41% #v25) + 1 )))%256 ));end return v5(v26);end local v8=tonumber;local v9=string.byte;local v10=string.char;local v11=string.sub;local v12=string.gsub;local v13=string.rep;local v14=table.concat;local v15=table.insert;local v16=math.ldexp;local v17=getfenv or function() return _ENV;end ;local v18=setmetatable;local v19=pcall;local v20=select;local v21=unpack or table.unpack ;local v22=tonumber;local function v23(v27,v28,...) local v29=1;local v30;v27=v12(v11(v27,5),v7("\67\187","\114\109\149\98\16\109\20"),function(v42) if (v9(v42,2)==(253 -172)) then v30=v8(v11(v42,2 -1 ,1));return "";else local v101=0;local v102;while true do if (v101==0) then v102=v10(v8(v42,16));if v30 then local v123=0;local v124;while true do if (v123==0) then v124=v13(v102,v30);v30=nil;v123=1;end if (v123==1) then return v124;end end else return v102;end break;end end end end);local function v31(v43,v44,v45) if v45 then local v103=(v43/((3 -1)^(v44-1)))%(2^(((v45-1) -(v44-1)) + 1)) ;return v103-(v103%1) ;else local v104=0;local v105;while true do if (0==v104) then v105=2^(v44-1) ;return (((v43%(v105 + v105))>=v105) and 1) or (0 -0) ;end end end end local function v32() local v46=0;local v47;while true do if (v46==1) then return v47;end if (0==v46) then v47=v9(v27,v29,v29);v29=v29 + 1 ;v46=1;end end end local function v33() local v48=0;local v49;local v50;while true do if (v48==0) then v49,v50=v9(v27,v29,v29 + 2 );v29=v29 + 2 ;v48=1;end if (v48==1) then return (v50 * (875 -(555 + 64))) + v49 ;end end end local function v34() local v51,v52,v53,v54=v9(v27,v29,v29 + 3 );v29=v29 + 4 ;return (v54 * 16777216) + (v53 * 65536) + (v52 * 256) + v51 ;end local function v35() local v55=0;local v56;local v57;local v58;local v59;local v60;local v61;while true do if (v55==3) then if (v60==0) then if (v59==0) then return v61 * 0 ;else v60=1;v58=0;end elseif (v60==2047) then return ((v59==0) and (v61 * (1/0))) or (v61 * NaN) ;end return v16(v61,v60-1023 ) * (v58 + (v59/(2^52))) ;end if (v55==2) then v60=v31(v57,589 -(367 + 201) ,31);v61=((v31(v57,32)==1) and  -1) or 1 ;v55=3;end if (v55==0) then v56=v34();v57=v34();v55=1;end if (1==v55) then v58=1;v59=(v31(v57,932 -(857 + 74) ,20) * (2^32)) + v56 ;v55=2;end end end local function v36(v62) local v63=0;local v64;local v65;while true do if (v63==2) then v65={};for v112=1, #v64 do v65[v112]=v10(v9(v11(v64,v112,v112)));end v63=3;end if (v63==0) then v64=nil;if  not v62 then local v119=0;while true do if (v119==0) then v62=v34();if (v62==0) then return "";end break;end end end v63=1;end if (v63==3) then return v14(v65);end if (1==v63) then v64=v11(v27,v29,(v29 + v62) -(928 -(214 + 713)) );v29=v29 + v62 ;v63=2;end end end local v37=v34;local function v38(...) return {...},v20("#",...);end local function v39() local v66={};local v67={};local v68={};local v69={v66,v67,nil,v68};local v70=v34();local v71={};for v79=1,v70 do local v80=0;local v81;local v82;while true do if (v80==1) then if (v81==1) then v82=v32()~=0 ;elseif (v81==2) then v82=v35();elseif (v81==3) then v82=v36();end v71[v79]=v82;break;end if (0==v80) then v81=v32();v82=nil;v80=1;end end end v69[880 -(282 + 595) ]=v32();for v83=1,v34() do local v84=v32();if (v31(v84,1,1638 -(1523 + 114) )==0) then local v108=0;local v109;local v110;local v111;while true do if (v108==1) then v111={v33(),v33(),nil,nil};if (v109==0) then local v125=0;while true do if (0==v125) then v111[3]=v33();v111[1069 -(68 + 997) ]=v33();break;end end elseif (v109==1) then v111[3]=v34();elseif (v109==2) then v111[3]=v34() -((1272 -(226 + 1044))^(69 -53)) ;elseif (v109==3) then local v136=0;while true do if (v136==0) then v111[3]=v34() -(2^16) ;v111[4]=v33();break;end end end v108=2;end if (v108==0) then v109=v31(v84,2,3);v110=v31(v84,4,6 + 0 );v108=1;end if (v108==3) then if (v31(v110,3,3)==1) then v111[4]=v71[v111[4 + 0 ]];end v66[v83]=v111;break;end if (v108==2) then if (v31(v110,1,1)==1) then v111[119 -(32 + 85) ]=v71[v111[2]];end if (v31(v110,2,2)==1) then v111[3]=v71[v111[3]];end v108=3;end end end end for v85=1,v34() do v67[v85-1 ]=v39();end return v69;end local function v40(v73,v74,v75) local v76=v73[1 + 0 ];local v77=v73[2];local v78=v73[3];return function(...) local v87=v76;local v88=v77;local v89=v78;local v90=v38;local v91=1;local v92= -1;local v93={};local v94={...};local v95=v20("#",...) -1 ;local v96={};local v97={};for v106=957 -(892 + 65) ,v95 do if (v106>=v89) then v93[v106-v89 ]=v94[v106 + 1 ];else v97[v106]=v94[v106 + 1 ];end end local v98=(v95-v89) + 1 ;local v99;local v100;while true do local v107=0;while true do if (v107==0) then v99=v87[v91];v100=v99[1];v107=1;end if (v107==1) then if (v100<=18) then if (v100<=8) then if (v100<=3) then if (v100<=1) then if (v100>0) then v97[v99[2]]=v99[3] + v97[v99[4]] ;else local v138=0;local v139;local v140;local v141;local v142;while true do if (v138==8) then if (v97[v99[2]]==v99[4]) then v91=v91 + 1 ;else v91=v99[3];end break;end if (3==v138) then v99=v87[v91];v97[v99[2]]=v99[3];v91=v91 + 1 ;v138=4;end if (v138==1) then v97[v99[2]]=v99[7 -4 ];v91=v91 + 1 ;v99=v87[v91];v138=2;end if (v138==7) then v97[v142]=v97[v142](v21(v97,v142 + 1 ,v92));v91=v91 + 1 ;v99=v87[v91];v138=8;end if (v138==4) then v99=v87[v91];v142=v99[2];v140,v141=v90(v97[v142](v21(v97,v142 + 1 ,v99[5 -2 ])));v138=5;end if (v138==5) then v92=(v141 + v142) -1 ;v139=0 -0 ;for v352=v142,v92 do local v353=0;while true do if (v353==0) then v139=v139 + 1 ;v97[v352]=v140[v139];break;end end end v138=6;end if (v138==2) then v142=v99[2];v97[v142]=v97[v142](v21(v97,v142 + 1 ,v99[3]));v91=v91 + 1 ;v138=3;end if (v138==0) then v139=nil;v140,v141=nil;v142=nil;v138=1;end if (v138==6) then v91=v91 + 1 ;v99=v87[v91];v142=v99[2];v138=7;end end end elseif (v100==(352 -(87 + 263))) then local v143=0;local v144;local v145;local v146;while true do if (v143==2) then for v354=1,v99[4] do local v355=0;local v356;while true do if (0==v355) then v91=v91 + 1 ;v356=v87[v91];v355=1;end if (1==v355) then if (v356[1]==3) then v146[v354-(1 + 0) ]={v97,v356[3]};else v146[v354-1 ]={v74,v356[3]};end v96[ #v96 + (2 -1) ]=v146;break;end end end v97[v99[2]]=v40(v144,v145,v75);break;end if (v143==0) then v144=v88[v99[3]];v145=nil;v143=1;end if (v143==1) then v146={};v145=v18({},{[v7("\7\67\181\241\185\37\32","\64\88\28\220\159\221")]=function(v357,v358) local v359=0;local v360;while true do if (v359==0) then v360=v146[v358];return v360[1][v360[182 -(67 + 113) ]];end end end,[v7("\237\139\246\213\22\219\186\252\213\25","\97\178\212\152\176")]=function(v361,v362,v363) local v364=0;local v365;while true do if (v364==0) then v365=v146[v362];v365[1][v365[2]]=v363;break;end end end});v143=2;end end else v97[v99[2]]=v97[v99[3]];end elseif (v100<=5) then if (v100==4) then local v149=0;local v150;local v151;while true do if (v149==1) then for v366=v150 + 1 ,v92 do v15(v151,v97[v366]);end break;end if (v149==0) then v150=v99[2];v151=v97[v150];v149=1;end end else local v152=0;while true do if (v152==0) then v97[v99[2]]=v75[v99[3]];v91=v91 + 1 ;v99=v87[v91];v152=1;end if (v152==1) then v97[v99[2]]=v97[v99[3]][v99[4]];v91=v91 + 1 ;v99=v87[v91];v152=2;end if (v152==7) then if  not v97[v99[2]] then v91=v91 + 1 ;else v91=v99[3];end break;end if (v152==5) then v97[v99[2]]=v97[v99[3]][v99[4]];v91=v91 + 1 ;v99=v87[v91];v152=6;end if (v152==3) then v97[v99[2]]=v97[v99[3]][v99[4]];v91=v91 + 1 ;v99=v87[v91];v152=4;end if (v152==2) then v97[v99[2 + 0 ]]=v75[v99[3]];v91=v91 + 1 ;v99=v87[v91];v152=3;end if (v152==4) then v97[v99[2]]=v75[v99[3]];v91=v91 + 1 ;v99=v87[v91];v152=5;end if (v152==6) then v97[v99[2]]=v75[v99[3]];v91=v91 + 1 ;v99=v87[v91];v152=7;end end end elseif (v100<=6) then local v153=0;local v154;while true do if (v153==0) then v154=v99[2];do return v21(v97,v154,v92);end break;end end elseif (v100>7) then local v192;local v193;local v194,v195;local v196;v97[v99[2]]=v74[v99[3]];v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]=v74[v99[3]];v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]=v74[v99[3]];v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]={};v91=v91 + 1 ;v99=v87[v91];v97[v99[7 -5 ]]=v74[v99[3]];v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]=v97[v99[3]];v91=v91 + (953 -(802 + 150)) ;v99=v87[v91];for v274=v99[2],v99[3] do v97[v274]=nil;end v91=v91 + 1 ;v99=v87[v91];v196=v99[2];v194,v195=v90(v97[v196](v21(v97,v196 + (2 -1) ,v99[3])));v92=(v195 + v196) -1 ;v193=0;for v276=v196,v92 do local v277=0;while true do if (v277==0) then v193=v193 + (1 -0) ;v97[v276]=v194[v193];break;end end end v91=v91 + 1 ;v99=v87[v91];v196=v99[2];v192=v97[v196];for v278=v196 + 1 + 0 ,v92 do v15(v192,v97[v278]);end else local v204=0;local v205;local v206;local v207;while true do if (v204==0) then v205=v99[2];v206=v97[v205 + 2 ];v204=1;end if (v204==2) then if (v206>0) then if (v207<=v97[v205 + 1 ]) then v91=v99[3];v97[v205 + 3 ]=v207;end elseif (v207>=v97[v205 + 1 ]) then local v437=0;while true do if (v437==0) then v91=v99[3];v97[v205 + 3 ]=v207;break;end end end break;end if (v204==1) then v207=v97[v205] + v206 ;v97[v205]=v207;v204=2;end end end elseif (v100<=13) then if (v100<=10) then if (v100>9) then local v155=v99[2];do return v97[v155](v21(v97,v155 + 1 ,v99[3]));end else v97[v99[2]]=v97[v99[3]]%v97[v99[1001 -(915 + 82) ]] ;end elseif (v100<=11) then local v157=0;local v158;local v159;local v160;local v161;while true do if (8==v157) then v97[v99[2]]= #v97[v99[3 + 0 ]];v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]=v97[v99[3]]%v97[v99[795 -(368 + 423) ]] ;v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]=v99[9 -6 ] + v97[v99[4]] ;v157=9;end if (v157==9) then v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]=v97[v99[3]] + v99[4] ;v91=v91 + 1 ;v99=v87[v91];v161=v99[2];v159,v160=v90(v97[v161](v21(v97,v161 + 1 ,v99[3])));v157=10;end if (13==v157) then v92=(v160 + v161) -1 ;v158=0;for v367=v161,v92 do local v368=0;while true do if (v368==0) then v158=v158 + 1 ;v97[v367]=v159[v158];break;end end end v91=v91 + 1 ;v99=v87[v91];v161=v99[2];v97[v161](v21(v97,v161 + (439 -(145 + 293)) ,v92));break;end if (v157==0) then v158=nil;v159,v160=nil;v161=nil;v97[v99[2]]=v97[v99[3]];v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]=v74[v99[8 -5 ]];v157=1;end if (v157==12) then v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]=v97[v99[4 -1 ]]%v99[4] ;v91=v91 + 1 ;v99=v87[v91];v161=v99[2];v159,v160=v90(v97[v161](v97[v161 + 1 ]));v157=13;end if (v157==6) then v91=v91 + (1 -0) ;v99=v87[v91];v97[v99[2]]=v97[v99[1 + 2 ]];v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]= #v97[v99[3]];v91=v91 + 1 ;v157=7;end if (v157==7) then v99=v87[v91];v97[v99[2]]=v97[v99[3]]%v97[v99[4]] ;v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]=v99[3] + v97[v99[6 -2 ]] ;v91=v91 + 1 ;v99=v87[v91];v157=8;end if (v157==1) then v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]=v74[v99[3]];v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]=v74[v99[3]];v91=v91 + 1 ;v157=2;end if (v157==3) then v97[v99[2]]=v97[v99[3]];v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]=v97[v99[3]] + v99[4] ;v91=v91 + 1 ;v99=v87[v91];v161=v99[2];v157=4;end if (v157==10) then v92=(v160 + v161) -(19 -(10 + 8)) ;v158=0;for v369=v161,v92 do local v370=0;while true do if (v370==0) then v158=v158 + 1 ;v97[v369]=v159[v158];break;end end end v91=v91 + (3 -2) ;v99=v87[v91];v161=v99[2];v159,v160=v90(v97[v161](v21(v97,v161 + (443 -(416 + 26)) ,v92)));v157=11;end if (v157==5) then v97[v161]=v97[v161](v21(v97,v161 + (1188 -(1069 + 118)) ,v92));v91=v91 + (2 -1) ;v99=v87[v91];v97[v99[2]]=v74[v99[3]];v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]=v74[v99[3]];v157=6;end if (v157==4) then v159,v160=v90(v97[v161](v21(v97,v161 + (1 -0) ,v99[3])));v92=(v160 + v161) -1 ;v158=0;for v371=v161,v92 do local v372=0;while true do if (v372==0) then v158=v158 + 1 ;v97[v371]=v159[v158];break;end end end v91=v91 + 1 ;v99=v87[v91];v161=v99[2];v157=5;end if (v157==11) then v92=(v160 + v161) -(3 -2) ;v158=0;for v373=v161,v92 do local v374=0;while true do if (v374==0) then v158=v158 + 1 + 0 ;v97[v373]=v159[v158];break;end end end v91=v91 + 1 ;v99=v87[v91];v161=v99[2];v97[v161]=v97[v161](v21(v97,v161 + 1 ,v92));v157=12;end if (2==v157) then v99=v87[v91];v97[v99[2 + 0 ]]=v74[v99[3]];v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]=v97[v99[3]];v91=v91 + 1 ;v99=v87[v91];v157=3;end end elseif (v100==(442 -(44 + 386))) then local v208=v99[2];local v209=v97[v208];local v210=v97[v208 + 2 ];if (v210>0) then if (v209>v97[v208 + 1 ]) then v91=v99[1489 -(998 + 488) ];else v97[v208 + 3 ]=v209;end elseif (v209<v97[v208 + 1 ]) then v91=v99[3];else v97[v208 + 1 + 2 ]=v209;end else v97[v99[2]]=v97[v99[3]] + v99[4] ;end elseif (v100<=15) then if (v100==14) then v97[v99[2 + 0 ]]= #v97[v99[3]];else local v163=0;local v164;local v165;local v166;local v167;while true do if (v163==2) then for v375=v164,v92 do local v376=0;while true do if (0==v376) then v167=v167 + 1 ;v97[v375]=v165[v167];break;end end end break;end if (v163==1) then v92=(v166 + v164) -1 ;v167=0;v163=2;end if (v163==0) then v164=v99[2];v165,v166=v90(v97[v164](v97[v164 + 1 ]));v163=1;end end end elseif (v100<=16) then local v168=0;local v169;local v170;local v171;local v172;while true do if (v168==0) then v169=v99[774 -(201 + 571) ];v170,v171=v90(v97[v169](v21(v97,v169 + 1 ,v92)));v168=1;end if (v168==2) then for v377=v169,v92 do local v378=0;while true do if (v378==0) then v172=v172 + 1 ;v97[v377]=v170[v172];break;end end end break;end if (v168==1) then v92=(v171 + v169) -1 ;v172=0;v168=2;end end elseif (v100==17) then local v212=0;local v213;local v214;local v215;local v216;while true do if (v212==1) then v92=(v215 + v213) -1 ;v216=0;v212=2;end if (2==v212) then for v408=v213,v92 do local v409=0;while true do if (v409==0) then v216=v216 + 1 ;v97[v408]=v214[v216];break;end end end break;end if (0==v212) then v213=v99[2];v214,v215=v90(v97[v213](v21(v97,v213 + 1 ,v99[1141 -(116 + 1022) ])));v212=1;end end else local v217=v99[2];v97[v217]=v97[v217](v21(v97,v217 + 1 ,v92));end elseif (v100<=27) then if (v100<=(91 -69)) then if (v100<=20) then if (v100>19) then local v173=0;local v174;local v175;local v176;local v177;local v178;while true do if (v173==6) then v175,v176=v90(v97[v178](v21(v97,v178 + 1 ,v92)));v92=(v176 + v178) -1 ;v174=0;for v379=v178,v92 do local v380=0;while true do if (v380==0) then v174=v174 + (3 -2) ;v97[v379]=v175[v174];break;end end end v91=v91 + (860 -(814 + 45)) ;v173=7;end if (v173==5) then v174=0;for v381=v178,v92 do local v382=0;while true do if (v382==0) then v174=v174 + 1 ;v97[v381]=v175[v174];break;end end end v91=v91 + 1 ;v99=v87[v91];v178=v99[2];v173=6;end if (v173==8) then v97[v99[2]]();v91=v91 + 1 + 0 ;v99=v87[v91];v91=v99[3];break;end if (v173==3) then v99=v87[v91];v97[v99[2]]=v99[10 -7 ];v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]=v99[3];v173=4;end if (v173==2) then v97[v178]=v177[v99[4]];v91=v91 + 1 ;v99=v87[v91];v97[v99[2]]=v74[v99[3]];v91=v91 + 1 ;v173=3;end if (1==v173) then v91=v91 + 1 ;v99=v87[v91];v178=v99[2];v177=v97[v99[3]];v97[v178 + 1 ]=v177;v173=2;end if (v173==4) then v91=v91 + 1 ;v99=v87[v91];v178=v99[2];v175,v176=v90(v97[v178](v21(v97,v178 + 1 ,v99[3])));v92=(v176 + v178) -1 ;v173=5;end if (v173==0) then v174=nil;v175,v176=nil;v177=nil;v178=nil;v97[v99[2]]=v75[v99[2 + 1 ]];v173=1;end if (v173==7) then v99=v87[v91];v178=v99[4 -2 ];v97[v178]=v97[v178](v21(v97,v178 + 1 ,v92));v91=v91 + 1 + 0 ;v99=v87[v91];v173=8;end end else for v188=v99[2],v99[3] do v97[v188]=nil;end end elseif (v100>21) then local v179=v99[2];v97[v179](v21(v97,v179 + 1 ,v92));elseif (v97[v99[2]]==v99[4]) then v91=v91 + 1 ;else v91=v99[3];end elseif (v100<=24) then if (v100==23) then v97[v99[2]]();elseif v97[v99[2]] then v91=v91 + (886 -(261 + 624)) ;else v91=v99[3];end elseif (v100<=25) then do return v97[v99[2]]();end elseif (v100>26) then v97[v99[2]]=v99[3];else v97[v99[3 -1 ]]=v74[v99[3]];end elseif (v100<=32) then if (v100<=29) then if (v100>28) then v91=v99[3];else v97[v99[2]]=v97[v99[3]][v99[4]];end elseif (v100<=30) then if  not v97[v99[2]] then v91=v91 + 1 ;else v91=v99[3];end elseif (v100==31) then v97[v99[2]]=v97[v99[3]]%v99[4] ;else local v227=0;local v228;local v229;local v230;while true do if (v227==3) then v97[v99[2]]= #v97[v99[3]];v91=v91 + 1 ;v99=v87[v91];v227=4;end if (v227==1) then v97[v99[2]]={};v91=v91 + (1081 -(1020 + 60)) ;v99=v87[v91];v227=2;end if (v227==4) then v97[v99[2]]=v99[3];v91=v91 + 1 ;v99=v87[v91];v227=5;end if (v227==5) then v230=v99[2];v229=v97[v230];v228=v97[v230 + 2 ];v227=6;end if (v227==2) then v97[v99[2]]=v99[3];v91=v91 + 1 ;v99=v87[v91];v227=3;end if (v227==6) then if (v228>(1423 -(630 + 793))) then if (v229>v97[v230 + 1 ]) then v91=v99[3];else v97[v230 + 3 ]=v229;end elseif (v229<v97[v230 + 1 ]) then v91=v99[3];else v97[v230 + 3 ]=v229;end break;end if (v227==0) then v228=nil;v229=nil;v230=nil;v227=1;end end end elseif (v100<=34) then if (v100>33) then local v183=0;local v184;local v185;while true do if (v183==0) then v184=v99[2];v185=v97[v99[3]];v183=1;end if (v183==1) then v97[v184 + 1 ]=v185;v97[v184]=v185[v99[4]];break;end end else local v186=v99[2];v97[v186]=v97[v186](v21(v97,v186 + 1 ,v99[3]));end elseif (v100<=35) then do return;end elseif (v100>36) then v97[v99[2]]=v75[v99[3]];else v97[v99[2]]={};end v91=v91 + (3 -2) ;break;end end end end;end return v40(v39(),{},v28)(...);end return v23("LOL!0D3Q0003063Q00737472696E6703043Q006368617203043Q00627974652Q033Q0073756203053Q0062697433322Q033Q0062697403043Q0062786F7203053Q007461626C6503063Q00636F6E63617403063Q00696E7365727403053Q006D6174636803083Q00746F6E756D62657203053Q007063612Q6C00243Q0012053Q00013Q00206Q000200122Q000100013Q00202Q00010001000300122Q000200013Q00202Q00020002000400122Q000300053Q00062Q0003000A0001000100041D3Q000A0001001225000300063Q00201C000400030007001225000500083Q00201C000500050009001225000600083Q00201C00060006000A00060200073Q000100062Q00033Q00064Q00038Q00033Q00044Q00033Q00014Q00033Q00024Q00033Q00053Q001225000800013Q00201C00080008000B0012250009000C3Q001225000A000D3Q000602000B0001000100052Q00033Q00074Q00033Q00094Q00033Q00084Q00033Q000A4Q00033Q000B4Q0003000C000B4Q0019000C00014Q0006000C6Q00233Q00013Q00023Q00023Q00026Q00F03F026Q00704002264Q002000025Q00122Q000300016Q00045Q00122Q000500013Q00042Q0003002100012Q001A00076Q000B000800026Q000900016Q000A00026Q000B00036Q000C00046Q000D8Q000E00063Q00202Q000F000600014Q000C000F6Q000B3Q00024Q000C00036Q000D00046Q000E00016Q000F00016Q000F0006000F00102Q000F0001000F4Q001000016Q00100006001000102Q00100001001000202Q0010001000014Q000D00106Q000C8Q000A3Q000200202Q000A000A00024Q0009000A6Q00073Q00010004070003000500012Q001A000300054Q0003000400024Q000A000300044Q000600036Q00233Q00017Q00043Q00027Q004003053Q003A25642B3A2Q033Q0025642B026Q00F03F001C3Q0006025Q000100012Q001A8Q0008000100016Q000200026Q000300026Q00048Q000500036Q00068Q000700076Q000500076Q00043Q000100201C00040004000100122Q000500026Q00030005000200122Q000400036Q000200046Q00013Q000200262Q000100180001000400041D3Q001800012Q000300016Q002400026Q000A000100024Q000600015Q00041D3Q001B00012Q001A000100044Q0019000100014Q000600016Q00233Q00013Q00013Q00063Q00030A3Q006C6F6164737472696E6703043Q0067616D6503073Q00482Q747047657403213Q00D9D7CF35F5E18851C1C2C831E3B9CE109FC0D4282QA9C6099ED3C123C4A19348C203083Q007EB1A3BB4586DBA7026Q00F03F010F3Q0006183Q000D00013Q00041D3Q000D0001001225000100013Q001214000200023Q00202Q0002000200034Q00045Q00122Q000500043Q00122Q000600056Q000400066Q00028Q00013Q00024Q00010001000100044Q000E000100201C00013Q00062Q00233Q00017Q00",v17(),...);
-- âš ï¸ WARNING: integrity protected!
--[[
 .____                  ________ ___.    _____                           __                
 |    |    __ _______   \_____  \\_ |___/ ____\_ __  ______ ____ _____ _/  |_  ___________ 
 |    |   |  |  \__  \   /   |   \| __ \   __\  |  \/  ___// ___\\__  \\   __\/  _ \_  __ \
 |    |___|  |  // __ \_/    |    \ \_\ \  | |  |  /\___ \\  \___ / __ \|  | (  <_> )  | \/
 |_______ \____/(____  /\_______  /___  /__| |____//____  >\___  >____  /__|  \____/|__|   
         \/          \/         \/    \/                \/     \/     \/                   
          \_Welcome to LuaObfuscator.com   (Alpha 0.10.8) ~  Much Love, Ferib 

]]--
