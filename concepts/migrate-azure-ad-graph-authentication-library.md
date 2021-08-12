---
title: Revisar alterações na biblioteca de autenticação de aplicativos
description: Descreve como atualizar o uso da biblioteca de autenticação para migrar um aplicativo de aplicativos da API Azure Active Directory (Azure AD) para a API Graph Microsoft.
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: f1b502c3d72fd194b809e355f09e43154ff5a4f27569c0fc534fcbfc55f11123
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163492"
---
# <a name="review-app-authentication-library-changes"></a>Revisar alterações na biblioteca de autenticação de aplicativos

Este artigo faz parte da *etapa 3:* revisar detalhes do aplicativo do [processo para migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)

A maioria dos aplicativos usa uma biblioteca de autenticação para adquirir e gerenciar tokens de acesso para chamar a Microsoft Graph.  A Microsoft oferece duas bibliotecas de autenticação:

- [Azure Active Directory biblioteca de autenticação](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL)
- [Biblioteca de autenticação da Microsoft](/azure/active-directory/develop/reference-v2-libraries) (MSAL)

## <a name="updating-adal"></a>Atualizando o ADAL

Se o aplicativo usa atualmente o ADAL, use uma abordagem de migração de dois estágios:

1. Atualize seu aplicativo para adquirir tokens de acesso para o Microsoft Graph. Continue a usar o ADAL para esta etapa. Atualize **o resourceURL**, que contém o URI que representa a API da Web de recursos, a partir de:

    `https://graph.windows.net`  

    Para:  

    `https://graph.microsoft.com`

    Tokens recém-adquiridos têm os mesmos escopos após essa alteração, mas o público-alvo dos tokens de acesso agora é o Microsoft Graph.  

    Depois de atualizar **resourceURL** e verificar a funcionalidade, libere uma atualização provisória para fazer com que os usuários se atualizem e executem.

1.  Em seguida, comece a trabalhar migrando seu aplicativo para usar o MSAL, que é a biblioteca com suporte para usar o avançar, agora que o ADAL está preterido.

## <a name="migrating-to-msal"></a>Migrando para o MSAL

O MSAL oferece vários benefícios sobre o ADAL, incluindo consentimento incremental, experiências de logom único mais ricas, suporte para contas pessoais da Microsoft, uso de protocolos baseados em padrões e assim por diante.  

Ao alternar seu aplicativo para o MSAL, você precisará fazer algumas alterações, incluindo a definição do parâmetro **scopes** na solicitação de aquisição de token:

``` csharp
var scopes = new string[] { "https://graph.microsoft.com/.default" };
```

A expressão acima limita a solicitação de escopos de permissão aos configurados durante o registro do aplicativo no Portal do Azure e salva seus usuários existentes de ter que consentir com seu aplicativo novamente.

Consulte [Migrando o ADAL para o MSAL](https://aka.ms/adal-net-to-msal-net) para ter ajuda direta e abrangente com o processo, incluindo solução de problemas e ajuda com erros comuns.

Depois de migrar para o MSAL, você pode solicitar escopos adicionais dinamicamente e os usuários são solicitados a fornecer consentimento incremental na próxima vez que usarem seu aplicativo.

## <a name="next-steps"></a>Próximos passos

- Saiba as diferenças de biblioteca de clientes do [.NET](migrate-azure-ad-graph-client-libraries.md) entre o Azure AD Graph e o Microsoft Graph.
- Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.