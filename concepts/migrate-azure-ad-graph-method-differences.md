---
title: Diferenças de método entre o Azure AD e o Microsoft Graph
description: Descreve as diferenças de método entre a API gráfica do Azure Active Directory (Azure AD) e a API do Microsoft Graph (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 95acfccc83fee798d5b06d78bbf10f02c128a640
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760669"
---
# <a name="method-differences-between-azure-ad-and-microsoft-graph"></a>Diferenças de método entre o Azure AD e o Microsoft Graph

Este artigo faz parte da *etapa 1: analisar as* diferenças de API do processo para [migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)

Alguns métodos do Azure AD Graph também foram alterados.  Se um método **não** for mostrado nesta lista, ele já estará disponível na versão [v1.0](/graph/api/overview?view=graph-rest-1.0) do Microsoft Graph, com exatamente o mesmo nome do Azure AD Graph.

|Azure AD Graph. <br>Método (v1.6) |Microsoft Graph<br>(recurso/método)|Comments|
|---|---|---|
| getAvailableExtensionProperties | beta &nbsp; - &nbsp; _Não disponível_ <br> v1.0 &nbsp; - &nbsp; [directoryObjects/getAvailableExtensionProperties](/graph/api/directoryobject-getavailableextensionproperties?view=graph-rest-1.0) |  |
| getObjectsByObjectId | beta &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-1.0) | |
| invalidateAllRefreshTokens | beta &nbsp; - &nbsp; [revogarSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [revogarSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) | |
| isMemberOf | beta &nbsp; - &nbsp; _Não planejado_ <br> v1.0 &nbsp; - &nbsp; _Não planejado_ | Use [checkMemberGroups.](/graph/api/user-checkmembergroups?view=graph-rest-1.0) |
| restore | restauração &nbsp; - &nbsp; [beta &nbsp; &nbsp; (aplicativos, usuários &nbsp; e &nbsp; grupos)](/graph/api/directory-deleteditems-restore?view=graph-rest-beta)<br> restauração v1.0 &nbsp; - &nbsp; [ &nbsp; (aplicativos, &nbsp; usuários &nbsp; e &nbsp; grupos)](/graph/api/directory-deleteditems-restore?view=graph-rest-1.0) | Você também pode exibir aplicativos, usuários e grupos excluídos e excluí-los permanentemente. |

## <a name="next-steps"></a>Próximas etapas

- Saiba como examinar [as diferenças de API em](migrate-azure-ad-graph-audit-api-use.md) seu aplicativo entre o Azure AD Graph e o Microsoft Graph.
- Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.
