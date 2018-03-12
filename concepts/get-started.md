# <a name="getting-started-building-microsoft-graph-apps"></a>Introdução à criação de aplicativos do Microsoft Graph

Os artigos desta seção fornecem orientações detalhadas sobre como criar aplicativos que se conectam ao Microsoft Graph em uma variedade de linguagens e plataformas de desenvolvimento. Cada artigo funciona como um projeto inicial e orienta você pelas etapas fundamentais para se conectar ao Microsoft Graph:

 1. Registrar o aplicativo
 2. Autenticar o usuário e obter um token de acesso no aplicativo
 3. Chamar o Microsoft Graph pelo aplicativo
 4. Executar o aplicativo

Se quiser uma solução de trabalho que entre em funcionamento mais rapidamente, experimente o [início rápido](https://developer.microsoft.com/graph/quick-start).

Cada projeto concluído é idêntico ao [Exemplo de conexão no repositório do Microsoft Graph](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) para essa plataforma.

Deseja ver ainda mais códigos?

Explore todos os [Exemplos do Microsoft Graph](https://github.com/microsoftgraph) no GitHub. A tabela a seguir mostra as versões adicionais dos exemplos abordados nesta seção. Elas demonstram como autenticar o usuário com os dois pontos de extremidade ADAL (v1.0 e v2.0) e usam as chamadas REST não processadas ou a biblioteca de cliente do Microsoft Graph (SDK) para se conectar ao Microsoft Graph.

Escolha o artigo correspondente ao provedor de autenticação e à plataforma de desenvolvimento de sua escolha e comece se conectando ao Microsoft Graph. Confira mais informações em [Qual é a diferença do ponto de extremidade v2.0?](https://docs.microsoft.com/pt-BR/azure/active-directory/develop/active-directory-v2-compare).


|Plataforma |Ponto de extremidade do Azure AD |Ponto de extremidade do Azure AD v2.0 |
|:--- |:--- |:---|
|Android |<a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">Exemplo de SDK</a> |<a href="https://github.com/microsoftgraph/android-java-connect-sample">Exemplo de SDK</a> ou <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">Exemplo de REST</a> |
|AngularJS |<a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a> |<a href="https://github.com/microsoftgraph/angular-connect-sample">Exemplo de SDK</a> ou <a href="https://github.com/microsoftgraph/angular-connect-rest-sample">Exemplo de REST</a> |
|ASP.NET |<a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a> |<a href="https://github.com/microsoftgraph/aspnet-connect-sample">Exemplo de SDK</a> ou <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">Exemplo de REST</a> |
|iOS (Obj-C) |<a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">Exemplo de REST</a> |<a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">Exemplo de SDK</a> |
|iOS (Swift) |<a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">Exemplo de REST</a> |<a href="https://github.com/microsoftgraph/ios-swift-connect-sample">Exemplo de SDK</a> |
|NodeJS |<a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a> |<a href="https://github.com/microsoftgraph/nodejs-connect-sample">Exemplo de SDK</a> ou <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">Exemplo de REST</a> |
|PHP |<a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a> |<a href="https://github.com/microsoftgraph/php-connect-sample">Exemplo de SDK</a> ou <a href="https://github.com/microsoftgraph/php-connect-rest-sample">Exemplo de REST</a> |
|Python |<a href="https://github.com/microsoftgraph/python-sample-auth/blob/master/sample_adal.py">Exemplo de REST</a> |<a href="https://aka.ms/graph-python-samples">Exemplo de REST</a>
|Ruby |<a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a> |<a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">Exemplo de REST</a> |
|UWP |<a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a> |<a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">Exemplo de SDK</a> ou <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">Exemplo de REST</a> |
|Xamarin | |<a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">Exemplo de SDK</a> |

<br/>

## <a name="see-also"></a>Confira também

- Experimente as chamadas REST de exemplo no [Explorador do Graph](https://developer.microsoft.com/pt-BR/graph/graph-explorer)
- [Documentação de ponto de extremidade do Microsoft Azure AD](https://docs.microsoft.com/pt-BR/azure/active-directory/develop/active-directory-developers-guide)
- [Documentação de ponto de extremidade do Azure AD v2.0](https://docs.microsoft.com/pt-BR/azure/active-directory/develop/active-directory-appmodel-v2-overview)
