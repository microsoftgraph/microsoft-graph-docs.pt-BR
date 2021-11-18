---
title: Diferenças de método entre o Azure AD Graph e o Microsoft Graph
description: Descreve as diferenças de método entre Azure Active Directory (Azure AD) Graph API e API Graph Microsoft (REST).
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: a9b9bdd59441f804a6a7314db3a1ae0a44d4cba7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077611"
---
# <a name="method-differences-between-azure-ad-graph-and-microsoft-graph"></a>Diferenças de método entre o Azure AD Graph e o Microsoft Graph

Este artigo faz parte da *etapa 1: analisar as* diferenças de API do processo para [migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)

Alguns métodos Azure Active Directory (Azure AD) Graph também foram alterados.  Se um  método não for mostrado nesta lista, ele já estará disponível na versão [v1.0](/graph/api/overview) do Microsoft Graph, com exatamente o mesmo nome do Azure AD Graph.

|Azure AD Graph. <br>Método (v1.6) |Microsoft Graph<br>(recurso/método)|Comentários|
|---|---|---|
| getAvailableExtensionProperties | beta &nbsp; - &nbsp; _Não disponível_ <br> v1.0 &nbsp; - &nbsp; [directoryObjects/getAvailableExtensionProperties](/graph/api/directoryobject-getavailableextensionproperties) |  |
| getObjectsByObjectId | beta &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-beta&preserve-view=true) <br> v1.0 &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids) | |
| invalidateAllRefreshTokens | beta &nbsp; - &nbsp; [revogarSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-beta&preserve-view=true) <br> v1.0 &nbsp; - &nbsp; [revogarSignInSessions](/graph/api/user-revokesigninsessions) | |
| isMemberOf | beta &nbsp; - &nbsp; _Não planejado_ <br> v1.0 &nbsp; - &nbsp; _Não planejado_ | Use [checkMemberGroups.](/graph/api/user-checkmembergroups) |
| restore | restauração &nbsp; - &nbsp; [beta &nbsp; &nbsp; (aplicativos, usuários &nbsp; e &nbsp; grupos)](/graph/api/directory-deleteditems-restore?view=graph-rest-beta&preserve-view=true)<br> restauração v1.0 &nbsp; - &nbsp; [ &nbsp; (aplicativos, &nbsp; usuários &nbsp; e &nbsp; grupos)](/graph/api/directory-deleteditems-restore) | Você também pode exibir aplicativos, usuários e grupos excluídos e excluí-los permanentemente. |

## <a name="next-steps"></a>Próximas etapas

- Saiba como examinar [as diferenças de API em](migrate-azure-ad-graph-audit-api-use.md) seu aplicativo entre o Azure AD Graph e o Microsoft Graph.
- Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.
