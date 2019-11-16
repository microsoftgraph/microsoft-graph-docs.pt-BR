---
title: Diferenças de métodos entre o Azure AD e o Microsoft Graph
description: Descreve as diferenças de métodos entre a API do Graph do Azure Active Directory (Azure AD) e a API do Microsoft Graph (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 00649e4f55a8bfcfd5354d2a75793447e3686109
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38656526"
---
# <a name="method-differences-between-azure-ad-and-microsoft-graph"></a>Diferenças de métodos entre o Azure AD e o Microsoft Graph

Este artigo faz parte da *etapa 1: revisar as diferenças de API* do [processo de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md).

Alguns métodos do Azure AD Graph também foram alterados.  Se um método **não** é mostrado na lista, ele já está disponível na [versão v 1.0](/graph/api/overview?view=graph-rest-1.0) do Microsoft Graph, com exatamente o mesmo nome que no Azure ad Graph.

|Azure AD Graph. <br>método (v 1.6) |Microsoft Graph<br>(recurso/método)|Comentários|
|---|---|---|
| getAvailableExtensionProperties | Beta- _não disponível_ <br> v 1.0- _não disponível_ |  |
| getObjectsByObjectId | diretório&nbsp;-&nbsp;beta/getByIds <br> v 1.0-Directory/getByIds | |
| invalidateAllRefreshTokens | Beta-revokeSignInSessions <br> v 1.0-revokeSignInSessions | |
| isMemberOf | Beta- _não planejado_ <br> v 1.0- _não planejado_ | Use checkMemberGroups em vez disso. |
| restore | &nbsp;-&nbsp;restauração&nbsp;beta (aplicativos,&nbsp;usuários&nbsp;e&nbsp;grupos)<br> &nbsp;-&nbsp;restauração&nbsp;de v 1.0 (&nbsp;usuários&nbsp;e grupos) | Você também pode exibir aplicativos, usuários e grupos excluídos e excluí-los permanentemente. |

## <a name="next-steps"></a>Próximos passos

- Saiba como [examinar as diferenças de API](migrate-azure-ad-graph-audit-api-use.md) em seu aplicativo entre o Azure ad Graph e o Microsoft Graph.
- Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .
- Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.
