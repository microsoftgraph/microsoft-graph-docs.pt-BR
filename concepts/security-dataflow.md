# <a name="microsoft-graph-security-data-flow"></a>Fluxo de dados do Microsoft Graph Security

A API do Microsoft Graph Security agrupa solicitações para todos os provedores no ecossistema do Microsoft Graph Security. Isso se baseia no consentimento de provedor de segurança fornecido pelo aplicativo, conforme mostrado no diagrama a seguir. O fluxo de trabalho de consentimento aplica-se somente a provedores não-Microsoft.

![security_dataflow_1.PNG](./images/security_dataflow_1.png)

A seguir, uma descrição do fluxo:

1. O usuário do aplicativo faz login no aplicativo do provedor para visualizar o formulário de consentimento do provedor. Esta experiência de formulário de consentimento ou interface do usuário é de propriedade do provedor e se aplica a provedores não Microsoft apenas para obter o consentimento explícito de seus clientes para enviar solicitações à API de segurança do Microsoft Graph.
2. O consentimento do cliente é armazenado no lado do provedor.
3. O serviço de consentimento do provedor chama a API de segurança do Microsoft Graph para informar a aprovação do consentimento para o respectivo cliente.
4. O aplicativo envia uma solicitação para a API de segurança do Microsoft Graph.
5. A API de segurança do Microsoft Graph verifica as informações de consentimento para esse cliente mapeadas para vários provedores.
6. A API de segurança do Microsoft Graph chama todos os provedores aos quais o cliente forneceu consentimento explícito por meio da experiência de consentimento do provedor.
7. A resposta é retornada de todos os provedores autorizados para esse cliente.
8. A resposta do conjunto de resultados é retornada para o aplicativo.
9. Se o cliente não tiver consentido em nenhum provedor, nenhum resultado desses fornecedores será incluído na resposta.
