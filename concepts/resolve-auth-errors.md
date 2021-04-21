---
title: Resolver erros de autorização do Microsoft Graph
description: Descubra como solucionar os erros de autorização do Microsoft Graph 401 e 403.
author: davidmu1
localization_priority: Priority
ms.prod: applications
ms.openlocfilehash: ecc8929c0671cbafed4baa5fc242a9f8515c7652
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921676"
---
# <a name="resolve-microsoft-graph-authorization-errors"></a>Resolver erros de autorização do Microsoft Graph

Erros de autorização podem ocorrer como resultado de vários problemas diferentes, a maioria dos quais gera um erro 403 (com algumas exceções). Por exemplo, todos os itens a seguir podem levar a erros de autorização:

* [Fluxos de aquisição de token de acesso](/azure/active-directory/develop/active-directory-authentication-scenarios) incorretos
* [Escopos de permissão](/azure/active-directory/develop/active-directory-v2-scopes) mal configurados
* Falta de [consentimento](/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)
* Falta de [permissões](/azure/active-directory/develop/v2-permissions-and-consent)

## <a name="steps-to-resolve-common-errors"></a>Etapas para resolver erros comuns

Para resolver erros de autorização comuns, experimente as etapas descritas para o erro que mais se aproxima do erro que está ocorrendo. Pode haver mais de um erro. Você também pode verificar as respostas já disponíveis no Microsoft Q&A para [401 erros](/answers/search.html?c=&f=&includeChildren=&q=%5bmicrosoft-graph%5d+401+&redirect=search%2fsearch&sort=relevance&type=question+OR+idea+OR+kbentry+OR+answer+OR+topic+OR+user) e [403 erros](/answers/search.html?c=&f=&includeChildren=&q=%5bmicrosoft-graph%5d+403&redirect=search%2fsearch&sort=relevance&type=question+OR+idea+OR+kbentry+OR+answer+OR+topic+OR+user). Se você não consegue encontrar uma solução para o seu problema, [faça uma nova pergunta no Microsoft Q&A](/answers/products/m365#microsoft-graph) e marcar com *microsoft-graph**.

**Erro 401 Não autorizado: seu token é válido?** <br>

Verifique se o seu aplicativo está apresentando um token de acesso válido ao Microsoft Graph como parte da solicitação. Esse erro geralmente significa que o token de acesso pode estar ausente no cabeçalho da solicitação de autenticação HTTP, ou que o token é inválido ou expirou. É altamente recomendável que você use a [Biblioteca de Autenticação da Microsoft (MSAL)](/azure/active-directory/develop/msal-overview) para aquisição de tokens de acesso. Além disso, esse erro pode ocorrer se você tentar usar um token de acesso delegado concedido a uma conta pessoal da Microsoft, para acessar uma API que só dê suporte a contas corporativas ou de estudante (contas organizacionais). 

**Erro 403 Proibido: você escolheu o conjunto certo de permissões?**<br>

Verifique se você solicitou o conjunto correto de permissões com base nas APIs do Microsoft Graph que seu aplicativo chama. As permissões menos privilegiadas que recomendamos são fornecidas em todos os tópicos de referência de método da API do Microsoft Graph. Além disso, essas permissões devem ser concedidas ao aplicativo por um usuário ou administrador. A concessão de permissões normalmente acontece por meio de uma página de consentimento, ou pela concessão de permissões usando a folha de registro do aplicativo Portal do Azure. Na folha **Configurações** do aplicativo, clique em **Permissões necessárias** e, em seguida, clique em **Conceder permissões**. <br>

* [Permissões do Microsoft Graph](./permissions-reference.md) <br>
* [Noções básicas sobre permissões e consentimento do Microsoft Azure Active Directory](/azure/active-directory/develop/v2-permissions-and-consent) <br>

**Erro 403 Proibido: seu aplicativo adquiriu um token para corresponder às permissões escolhidas?** <br>

Certifique-se de que o tipo de permissão solicitado ou concedido corresponda ao tipo de token de acesso que seu aplicativo adquire. Você pode estar solicitando e concedendo permissões do aplicativo, mas usando tokens de fluxo de código interativo delegados, em vez de tokens de fluxo de credencial de cliente, ou solicitando e concedendo permissões delegadas, mas usando tokens de fluxo de credenciais de cliente em vez de tokens de fluxo de código delegados. <br>
* [Obtenha acesso em nome de usuários e permissões delegadas](/graph/auth_v2_user) 
* [Azure AD v2.0 - fluxo de código de autorização OAuth 2.0](/azure/active-directory/develop/v2-oauth2-auth-code-flow)
* [Obter acesso sem um usuário (serviço daemon) e permissões de aplicativo](/graph/auth_v2_service)
* [Azure AD v2.0 - fluxo de credenciais do cliente OAuth 2.0](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**Erro 403 Proibido: redefinindo a senha** <br>

No momento, não há permissões de serviço a serviço de permissão de aplicativo daemon que permitam a redefinição de senhas dos usuários. Essas APIs têm suporte somente usando os fluxos de código delegados interativos com um administrador conectado.

* [Permissões do Microsoft Graph](./permissions-reference.md) <br>

**403 Proibido: o usuário tem acesso e está licenciado?** <br>

Para fluxos de código delegados, o Microsoft Graph avalia se a solicitação é permitida com base nas permissões concedidas ao aplicativo e nas permissões que o usuário conectado possui. Geralmente, esse erro indica que o usuário não tem privilégio suficiente para executar a solicitação **ou** não está licenciado para os dados que estão sendo acessados. Somente os usuários com as permissões ou licenças necessárias podem fazer a solicitação com êxito.

**403 Proibido: você selecionou a API de recurso correta?** <br>

Serviços de API como o Microsoft Graph verificam se a declaração *aud* (audiência) no token de acesso recebido corresponde ao valor esperado para si e, caso contrário, resultam em um erro `403 Forbidden`. Um equívoco comum que causa esse erro é tentar usar um token adquirido para APIs do Microsoft Graph, APIs do Outlook ou APIs do SharePoint/OneDrive do Azure AD para chamar o Microsoft Graph (ou vice-versa). Verifique se o recurso (ou escopo) para o qual o seu aplicativo está adquirindo um token corresponde à API que o aplicativo está chamando.

**400 Solicitação incorreta ou 403 Proibido: o usuário está em conformidade com as políticas de acesso condicional (CA) da organização?**<br>

Com base nas políticas de CA de uma organização, um usuário que acessa os recursos do Microsoft Graph por meio do seu aplicativo pode ser desafiado a obter informações adicionais que não estão presentes no token de acesso que o aplicativo adquiriu originalmente. Nesse caso, seu aplicativo recebe um 400 com um erro *interaction_required* durante a aquisição de token de acesso, ou um 403 com o erro *insufficient_claims* ao chamar o Microsoft Graph. Em ambos os casos, a resposta ao erro contém informações adicionais que podem ser apresentadas ao ponto de extremidade de autorização para desafiar o usuário a obter informações adicionais (como autenticação multifator ou registro do dispositivo).

* [Lidar com desafios de acesso condicional usando a MSAL](/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
* [Orientações do desenvolvedor para acesso condicional do Azure Active Directory](/azure/active-directory/develop/conditional-access-dev-guide)
