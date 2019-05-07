---
title: Analisar alterações da biblioteca de autenticação do aplicativo
description: Descreve como atualizar o uso da biblioteca de autenticação para migrar um aplicativo dos aplicativos de API do Azure Active Directory (Azure AD) para a API do Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 77604945064565f1387553b22a26a0fa871c998d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630262"
---
# <a name="review-app-authentication-library-changes"></a>Analisar alterações da biblioteca de autenticação do aplicativo

Este artigo faz parte da *etapa 3: revise os detalhes do aplicativo* do [processo para migrar aplicativos](migrate-azure-ad-graph-planning-checklist.md).

A maioria dos aplicativos usa uma biblioteca de autenticação para aquire e gerenciar tokens de acesso para chamar o Microsoft Graph.  A Microsoft oferece duas bibliotecas de autenticação:

- [Biblioteca de autenticação do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) Adal
- [Biblioteca de autenticação da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) MSAL

## <a name="updating-adal"></a>Atualizando ADAL

Se seu aplicativo usa atualmente a ADAL, use uma abordagem de migração de dois estágios:

1. Atualize seu aplicativo para adquirir tokens de acesso para o Microsoft Graph. Continue a usar a ADAL para esta etapa. Atualize o **resourceurl pela**, que contém o URI que representa a API Web de recurso, de:

    `https://graph.windows.net`  

    Para:  

    `https://graph.microsoft.com`

    Tokens adquiridos recentemente têm os mesmos escopos após essa alteração, mas a audiência dos tokens de acesso agora é o Microsoft Graph.  

    Após a atualização do **resourceurl pela** e verificação da funcionalidade, libere uma atualização provisória para que seus usuários sejam ativados e runnning.

1.  Em seguida, comece a migrar o aplicativo para usar o MSAL, que é a biblioteca com suporte para usar a movimentação para frente.

## <a name="migrating-to-msal"></a>Migrando para o MSAL

O MSAL fornece vários benefícios sobre a ADAL, incluindo o consentimento incremental, experiências de logon único mais ricas, suporte para contas pessoais da Microsoft, uso de protocolos baseados em padrões e assim por diante.  

Ao mudar seu aplicativo para o MSAL, você precisará fazer algumas alterações, incluindo a configuração do parâmetro de **** escopos na solicitação de token Acquistion:

``` csharp
var scopes = new string[] { "https://graph.microsoft.com/.default" };
```

A expressão acima limita a solicitação de escopos de permissão para aquelas configuradas durante o registro do aplicativo no portal do Azure e salva seus usuários existentes para que eles tenham de ser consentidos em seu aplicativo novamente.

Consulte [migraNDO Adal para MSAL](https://aka.ms/adal-net-to-msal-net) para obter ajuda direta e abrangente com o processo, incluindo solução de problemas e ajuda com erros comuns.

Após a migração para o MSAL, você poderá solicitar escopos adicionais dinamicamente e os usuários serão solicitados a fornecer o consentimento incremental na próxima vez que usarem seu aplicativo.

## <a name="next-steps"></a>Próximos passos

- Saiba mais sobre as diferenças de [biblioteca de cliente .net](migrate-azure-ad-graph-client-libraries.md) entre o Azure AD e o Microsoft Graph.
- Explore a [migração de Adal para o MSAL](https://aka.ms/adal-net-to-msal-net) para obter ajuda mais detalhada sobre a migração para o MSAL.
- Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .
- Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.
