# transfer-learning-pytorch

For fun, how I've used the "Transfer Learning" capability of PyTorch to resolve the challenge at:<br />
https://github.com/EvilRobotOverlord/huedump

Or, from this gif picture (37 frames):<br />
![gif picture](https://github.com/STPR/transfer-learning-pytorch/blob/master/original.gif)

To this text:<br />
``EFBBBF2F2F20467574757265``<br />
``2076657273696F6E73206F66``<br />
``204879706572206D61792061``<br />
``6464206164646974696F6E61``<br />
``6C20636F6E666967206F7074``<br />
``696F6E732C0D0A2F2F207768``<br />
``6963682077696C6C206E6F74``<br />
``206175746F6D61746963616C``<br />
``6C79206265206D6572676564``<br />
``20696E746F20746869732066``<br />
``696C652E0D0A2F2F20536565``<br />
``2068747470733A2F2F687970``<br />
``65722E69732363666720666F``<br />
``7220616C6C2063757272656E``<br />
``746C7920737570706F727465``<br />
``64206F7074696F6E732E0D0A``<br />
``0D0A6D6F64756C652E657870``<br />
``6F727473203D207B0D0A2020``<br />
``636F6E6669673A207B0D0A20``<br />
``2020202F2F2063686F6F7365``<br />
``206569746865722060277374``<br />
``61626C65276020666F722072``<br />
``6563656976696E6720686967``<br />
``686C7920706F6C6973686564``<br />
``2C0D0A202020202F2F206F72``<br />
``20602763616E617279276020``<br />
``666F72206C65737320706F6C``<br />
``697368656420627574206D6F``<br />
``7265206672657175656E7420``<br />
``757064617465730D0A202020``<br />
``207570646174654368616E6E``<br />
``656C3A2027737461626C6527``<br />
``2C0D0A0D0A202020202F2F20``<br />
``64656661756C7420666F6E74``<br />
``2073697A6520696E20706978``<br />
``656C7320666F7220616C6C20``<br />
``746162730D0A20202020666F``<br />
``6E7453697A653A2031322C0D``<br />
``0A0D0A202020202F2F20666F``<br />
``6E742066616D696C79207769``<br />
``7468206F7074696F6E616C20``<br />
``66616C6C6261636B730D0A20``<br />
``202020666F6E7446616D696C``<br />
``793A2027496E636F6E736F6C``<br />
``6174612C204D656E6C6F2C20``<br />
``2244656A6156752053616E73``<br />
``204D6F6E6F222C20436F6E73``<br />
``6F6C61732C20224C75636964``<br />
``6120436F6E736F6C65222C20``<br />
``6D6F6E6F7370616365272C0D``<br />
``0A0D0A202020202F2F206465``<br />
``6661756C7420666F6E742077``<br />
``65696768743A20276E6F726D``<br />
``616C27206F722027626F6C64``<br />
``270D0A20202020666F6E7457``<br />
``65696768743A20276E6F726D``<br />
``616C272C0D0A0D0A20202020``<br />
``2F2F20666F6E742077656967``<br />
``687420666F7220626F6C6420``<br />
``636861726163746572733A20``<br />
``276E6F726D616C27206F7220``<br />
``27626F6C64270D0A20202020``<br />
``666F6E74576569676874426F``<br />
``6C643A2027626F6C64272C0D``<br />
``0A0D0A202020202F2F207465``<br />
``726D696E616C20637572736F``<br />
``72206261636B67726F756E64``<br />
``20636F6C6F7220616E64206F``<br />
``70616369747920286865782C``<br />
``207267622C2068736C2C2068``<br />
``73762C20687762206F722063``<br />
``6D796B290D0A202020206375``<br />
``72736F72436F6C6F723A2027``<br />
``72676261283234382C32382C``<br />
``3232392C302E3829272C0D0A``<br />
``0D0A202020202F2F20746572``<br />
``6D696E616C20746578742063``<br />
``6F6C6F7220756E6465722042``<br />
``4C4F434B20637572736F720D``<br />
``0A20202020637572736F7241``<br />
``6363656E74436F6C6F723A20``<br />
``2723303030272C0D0A0D0A20``<br />
``2020202F2F2060274245414D``<br />
``276020666F72207C2C206027``<br />
``554E4445524C494E45276020``<br />
``666F72205F2C206027424C4F``<br />
``434B276020666F7220E29688``<br />
``0D0A20202020637572736F72``<br />
``53686170653A20274245414D``<br />
``272C0D0A0D0A202020202F2F``<br />
``2073657420746F2060747275``<br />
``65602028776974686F757420``<br />
``6261636B7469636B7320616E``<br />
``6420776974686F7574207175``<br />
``6F7465732920666F7220626C``<br />
``696E6B696E6720637572736F``<br />
``720D0A20202020637572736F``<br />
``72426C696E6B3A2074727565``<br />
``2C0D0A0D0A202020202F2F20``<br />
``636F6C6F72206F6620746865``<br />
``20746578740D0A2020202066``<br />
``6F726567726F756E64436F6C``<br />
``6F723A202723666666272C0D``<br />
``0A0D0A202020202F2F207465``<br />
``726D696E616C206261636B67``<br />
``726F756E6420636F6C6F720D``<br />
``0A202020202F2F206F706163``<br />
``697479206973206F6E6C7920``<br />
``737570706F72746564206F6E``<br />
``206D61634F530D0A20202020``<br />
``6261636B67726F756E64436F``<br />
``6C6F723A202723303030272C``<br />
``0D0A0D0A202020202F2F2074``<br />
``65726D696E616C2073656C65``<br />
``6374696F6E20636F6C6F720D``<br />
``0A2020202073656C65637469``<br />
``6F6E436F6C6F723A20277267``<br />
``6261283234382C32382C3232``<br />
``392C302E3329272C0D0A0D0A``<br />
``202020202F2F20626F726465``<br />
``7220636F6C6F72202877696E``<br />
``646F772C2074616273290D0A``<br />
``20202020626F72646572436F``<br />
``6C6F723A202723333333272C``<br />
``0D0A0D0A202020202F2F2063``<br />
``7573746F6D2043535320746F``<br />
``20656D62656420696E207468``<br />
``65206D61696E2077696E646F``<br />
``770D0A202020206373733A20``<br />
``27272C0D0A0D0A202020202F``<br />
``2F20637573746F6D20435353``<br />
``20746F20656D62656420696E``<br />
``20746865207465726D696E61``<br />
``2073686F77206E6174697665``<br />
``206D656E75732C2073657420``<br />
``746F2066616C73650D0A2020``<br />
``20202F2F2064656661756C74``<br />
``3A20607472756560206F6E20``<br />
``4C696E75782C206074727565``<br />
``60206F6E2057696E646F7773``<br />
``2C2069676E6F726564206F6E``<br />
``206D61634F530D0A20202020``<br />
``73686F7748616D6275726765``<br />
``724D656E753A2027272C0D0A``<br />
``0D0A202020202F2F20736574``<br />
``20746F206066616C73656020``<br />
``28776974686F757420626163``<br />
``6B7469636B7320616E642077``<br />
``6974686F75742071756F7465``<br />
``732920696620796F75207761``<br />
``6E7420746F20686964652074``<br />
``6865206D696E696D697A652C``<br />
``206D6178696D697A6520616E``<br />
``6420636C6F73652062757474``<br />
``6F6E730D0A202020202F2F20``<br />
``6164646974696F6E616C6C79``<br />
``2C2073657420746F2060276C``<br />
``656674276020696620796F75``<br />
``2077616E74207468656D206F``<br />
``6E20746865206C6566742C20``<br />
``6C696B6520696E205562756E``<br />
``74750D0A202020202F2F2064``<br />
``656661756C743A2060747275``<br />
``65602028776974686F757420``<br />
``6261636B7469636B7320616E``<br />
``6420776974686F7574207175``<br />
``6F74657329206F6E2057696E``<br />
``646F777320616E64204C696E``<br />
``75782C2069676E6F72656420``<br />
``6F6E206D61634F530D0A2020``<br />
``202073686F7757696E646F77``<br />
``436F6E74726F6C733A202727``<br />
``2C0D0A0D0A202020202F2F20``<br />
``637573746F6D207061646469``<br />
``6E67202843535320666F726D``<br />
``61742C20692E652E3A206074``<br />
``6F7020726967687420626F74``<br />
``746F6D206C65667460290D0A``<br />
``2020202070616464696E673A``<br />
``202731327078203134707827``<br />
``2C0D0A0D0A202020202F2F20``<br />
``7468652066756C6C206C6973``<br />
``742E20696620796F75277265``<br />
``20676F696E6720746F207072``<br />
``6F7669646520746865206675``<br />
``6C6C20636F6C6F722070616C``<br />
``657474652C0D0A202020202F``<br />
``2F20696E636C7564696E6720``<br />
``74686520362078203620636F``<br />
``6C6F7220637562657320616E``<br />
``642074686520677261797363``<br />
``616C65206D61702C206A7573``<br />
``742070726F766964650D0A20``<br />
``2020202F2F20616E20617272``<br />
``6179206865726520696E7374``<br />
``656164206F66206120636F6C``<br />
``6F72206D6170206F626A6563``<br />
``740D0A20202020636F6C6F72``<br />
``733A207B0D0A202020202020``<br />
``626C61636B3A202723303030``<br />
``303030272C0D0A2020202020``<br />
``207265643A20272343353145``<br />
``3134272C0D0A202020202020``<br />
``677265656E3A202723314443``<br />
``313231272C0D0A2020202020``<br />
``2079656C6C6F773A20272343``<br />
``3743333239272C0D0A202020``<br />
``202020626C75653A20272330``<br />
``4132464334272C0D0A202020``<br />
``2020206D6167656E74613A20``<br />
``2723433833394335272C0D0A``<br />
``2020202020206379616E3A20``<br />
``2723323043354336272C0D0A``<br />
``20202020202077686974653A``<br />
``202723433743374337272C0D``<br />
``0A2020202020206C69676874``<br />
``426C61636B3A202723363836``<br />
``383638272C0D0A2020202020``<br />
``206C696768745265643A2027``<br />
``23464436463642272C0D0A20``<br />
``20202020206C696768744772``<br />
``65656E3A2027233637463836``<br />
``46272C0D0A2020202020206C``<br />
``6967687459656C6C6F773A20``<br />
``2723464646413732272C0D0A``<br />
``2020202020206C6967687442``<br />
``6C75653A2027233641373646``<br />
``42272C0D0A2020202020206C``<br />
``696768744D6167656E74613A``<br />
``202723464437434643272C0D``<br />
``0A2020202020206C69676874``<br />
``4379616E3A20272336384644``<br />
``4645272C0D0A202020202020``<br />
``6C6967687457686974653A20``<br />
``2723464646464646272C0D0A``<br />
``202020207D2C0D0A0D0A2020``<br />
``20202F2F2074686520736865``<br />
``6C6C20746F2072756E207768``<br />
``656E20737061776E696E6720``<br />
``61206E65772073657373696F``<br />
``6E2028692E652E202F757372``<br />
``2F6C6F63616C2F62696E2F66``<br />
``697368290D0A202020202F2F``<br />
``206966206C65667420656D70``<br />
``74792C20796F757220737973``<br />
``74656D2773206C6F67696E20``<br />
``7368656C6C2077696C6C2062``<br />
``652075736564206279206465``<br />
``6661756C740D0A202020202F``<br />
``2F0D0A202020202F2F205769``<br />
``6E646F77730D0A202020202F``<br />
``2F202D204D616B6520737572``<br />
``6520746F2075736520612066``<br />
``756C6C207061746820696620``<br />
``7468652062696E617279206E``<br />
``616D6520646F65736E277420``<br />
``776F726B0D0A202020202F2F``<br />
``202D2052656D6F766520602D``<br />
``2D6C6F67696E6020696E2073``<br />
``68656C6C417267730D0A2020``<br />
``20202F2F0D0A202020202F2F``<br />
``2042617368206F6E2057696E``<br />
``646F77730D0A202020202F2F``<br />
``202D204578616D706C653A20``<br />
``60433A5C5C57696E646F7773``<br />
``5C5C53797374656D33325C5C``<br />
``626173682E657865600D0A20``<br />
``2020202F2F0D0A202020202F``<br />
``2F20506F7765725368656C6C``<br />
``206F6E2057696E646F77730D``<br />
``0A202020202F2F202D204578``<br />
``616D706C653A2060433A5C5C``<br />
``57494E444F57535C5C537973``<br />
``74656D33325C5C57696E646F``<br />
``7773506F7765725368656C6C``<br />
``5C5C76312E305C5C706F7765``<br />
``727368656C6C2E657865600D``<br />
``0A202020207368656C6C3A20``<br />
``27433A5C5C57696E646F7773``<br />
``5C5C53797374656D33325C5C``<br />
``57696E646F7773506F776572``<br />
``5368656C6C5C5C76312E305C``<br />
``5C706F7765727368656C6C2E``<br />
``657865272C0D0A0D0A202020``<br />
``202F2F20666F722073657474``<br />
``696E67207368656C6C206172``<br />
``67756D656E74732028692E65``<br />
``2E20666F72207573696E6720``<br />
``696E74657261637469766520``<br />
``7368656C6C417267733A2060``<br />
``5B272D69275D60290D0A2020``<br />
``20202F2F2062792064656661``<br />
``756C7420605B272D2D6C6F67``<br />
``696E275D602077696C6C2062``<br />
``6520757365640D0A20202020``<br />
``7368656C6C417267733A205B``<br />
``27275D2C0D0A0D0A20202020``<br />
``2F2F20666F7220656E766972``<br />
``6F6E6D656E74207661726961``<br />
``626C65730D0A20202020656E``<br />
``763A207B7D2C0D0A0D0A2020``<br />
``20202F2F2073657420746F20``<br />
``6066616C73656020666F7220``<br />
``6E6F2062656C6C0D0A202020``<br />
``2062656C6C3A2027534F554E``<br />
``44272C0D0A0D0A202020202F``<br />
``2F2069662060747275656020``<br />
``28776974686F757420626163``<br />
``6B7469636B7320616E642077``<br />
``6974686F75742071756F7465``<br />
``73292C2073656C6563746564``<br />
``20746578742077696C6C2061``<br />
``75746F6D61746963616C6C79``<br />
``20626520636F706965642074``<br />
``6F2074686520636C6970626F``<br />
``6172640D0A20202020636F70``<br />
``794F6E53656C6563743A2066``<br />
``616C73652C0D0A0D0A202020``<br />
``202F2F206966206074727565``<br />
``602028776974686F75742062``<br />
``61636B7469636B7320616E64``<br />
``20776974686F75742071756F``<br />
``746573292C20687970657220``<br />
``77696C6C2062652073657420``<br />
``617320746865206465666175``<br />
``6C742070726F746F636F6C20``<br />
``636C69656E7420666F722053``<br />
``53480D0A2020202064656661``<br />
``756C745353484170703A2074``<br />
``7275652C0D0A0D0A20202020``<br />
``2F2F20696620607472756560``<br />
``2028776974686F7574206261``<br />
``636B7469636B7320616E6420``<br />
``776974686F75742071756F74``<br />
``6573292C206F6E2072696768``<br />
``7420636C69636B2073656C65``<br />
``637465642074657874207769``<br />
``6C6C20626520636F70696564``<br />
``206F72207061737465642069``<br />
``66206E6F0D0A202020202F2F``<br />
``2073656C656374696F6E2069``<br />
``732070726573656E74202860``<br />
``747275656020627920646566``<br />
``61756C74206F6E2057696E64``<br />
``6F777320616E642064697361``<br />
``626C65732074686520636F6E``<br />
``74657874206D656E75206665``<br />
``6174757265290D0A20202020``<br />
``2F2F20717569636B45646974``<br />
``3A20747275652C0D0A0D0A20``<br />
``2020202F2F2055524C20746F``<br />
``20637573746F6D2062656C6C``<br />
``0D0A202020202F2F2062656C``<br />
``6C536F756E6455524C3A2027``<br />
``687474703A2F2F6578616D70``<br />
``6C652E636F6D2F62656C6C2E``<br />
``6D7033272C0D0A0D0A202020``<br />
``202F2F20666F722061647661``<br />
``6E63656420636F6E66696720``<br />
``666C61677320706C65617365``<br />
``20726566657220746F206874``<br />
``7470733A2F2F68797065722E``<br />
``69732F236366670D0A20207D``<br />
``2C0D0A0D0A20202F2F206120``<br />
``6C697374206F6620706C7567``<br />
``696E7320746F206665746368``<br />
``20616E6420696E7374616C6C``<br />
``2066726F6D206E706D0D0A20``<br />
``202F2F20666F726D61743A20``<br />
``5B406F72672F5D70726F6A65``<br />
``63745B2376657273696F6E5D``<br />
``0D0A20202F2F206578616D70``<br />
``6C65733A0D0A20202F2F2020``<br />
``20606879706572706F776572``<br />
``600D0A20202F2F2020206040``<br />
``636F6D70616E792F70726F6A``<br />
``656374600D0A20202F2F2020``<br />
``206070726F6A65637423312E``<br />
``302E31600D0A2020706C7567``<br />
``696E733A205B0D0A20202020``<br />
``2768797065726C696E6B7327``<br />
``2C0D0A202020202768797065``<br />
``722D7374617475736C696E65``<br />
``272C0D0A2020202027687970``<br />
``65722D6D6174657269616C2D``<br />
``7468656D65270D0A20205D2C``<br />
``0D0A0D0A20202F2F20696E20``<br />
``646576656C6F706D656E742C``<br />
``20796F752063616E20637265``<br />
``617465206120646972656374``<br />
``6F727920756E6465720D0A20``<br />
``202F2F20607E2F2E68797065``<br />
``725F706C7567696E732F6C6F``<br />
``63616C2F6020616E6420696E``<br />
``636C75646520697420686572``<br />
``650D0A20202F2F20746F206C``<br />
``6F616420697420616E642061``<br />
``766F6964206974206265696E``<br />
``6720606E706D20696E737461``<br />
``6C6C6065640D0A20206C6F63``<br />
``616C506C7567696E733A205B``<br />
``5D2C0D0A0D0A20206B65796D``<br />
``6170733A207B0D0A20202020``<br />
``2F2F204578616D706C650D0A``<br />
``202020202F2F202777696E64``<br />
``6F773A646576746F6F6C7327``<br />
``3A2027636D642B616C742B6F``<br />
``272C0D0A20207D2C0D0A7D3B``<br />
``0D0A``<br />
