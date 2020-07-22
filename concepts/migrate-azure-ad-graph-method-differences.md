---
title: Diferenças de métodos entre o Azure AD e o Microsoft Graph
description: Descreve as diferenças de métodos entre a API do Graph do Azure Active Directory (Azure AD) e a API do Microsoft Graph (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 515c08913cac522b9b920032fe32912eb7bfd25f
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45224868"
---
# <a name="method-differences-between-azure-ad-and-microsoft-graph"></a>Diferenças de métodos entre o Azure AD e o Microsoft Graph

Este artigo faz parte da *etapa 1: revisar as diferenças de API* do [processo de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md).

Alguns métodos do Azure AD Graph também foram alterados.  Se um método **não** é mostrado na lista, ele já está disponível na [versão v 1.0](/graph/api/overview?view=graph-rest-1.0) do Microsoft Graph, com exatamente o mesmo nome que no Azure ad Graph.

|Azure AD Graph. <br>método (v 1.6) |Microsoft Graph<br>(recurso/método)|Comentários|
|---|---|---|
| getAvailableExtensionProperties | versão beta &nbsp; - &nbsp; _não disponível_ <br> v 1.0 &nbsp; - &nbsp; [directoryObjects/getAvailableExtensionProperties](/graph/api/directoryobject-getavailableextensionproperties?view=graph-rest-1.0) |  |
| getObjectsByObjectId | versão beta &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-beta) <br> v 1.0 &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-1.0) | |
| invalidateAllRefreshTokens | versão beta &nbsp; - &nbsp; [revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-beta) <br> v 1.0 &nbsp; - &nbsp; [revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) | |
| isMemberOf | versão beta &nbsp; - &nbsp; _não planejada_ <br> v 1.0 &nbsp; - &nbsp; _não planejado_ | Use checkMemberGroups em vez disso. |
| restore | &nbsp; - &nbsp; [restauração beta &nbsp; (aplicativos, &nbsp; usuários &nbsp; e &nbsp; grupos)](/graph/api/directory-deleteditems-restore?view=graph-rest-beta)<br> v 1.0 &nbsp; - &nbsp; [Restore &nbsp; (aplicativos, &nbsp; usuários &nbsp; e &nbsp; grupos)](/graph/api/directory-deleteditems-restore?view=graph-rest-1.0) | Você também pode exibir aplicativos, usuários e grupos excluídos e excluí-los permanentemente. |

## <a name="next-steps"></a>Próximas etapas

- Saiba como [examinar as diferenças de API](migrate-azure-ad-graph-audit-api-use.md) em seu aplicativo entre o Azure ad Graph e o Microsoft Graph.
- Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .
- Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.
