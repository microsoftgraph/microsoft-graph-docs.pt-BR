---
title: Diferenças de método entre Azure Active Directory (Azure AD) Graph Microsoft Graph
description: Descreve as diferenças de método entre Azure Active Directory (Azure AD) Graph API e API Graph Microsoft (REST).
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: fab1da340ca4a7703f2434f0d3a30b8e1b08821d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139090"
---
# <a name="method-differences-between-azure-active-directory-azure-ad-and-microsoft-graph"></a>Diferenças de método entre Azure Active Directory (Azure AD) e Microsoft Graph

Este artigo faz parte da *etapa 1: analisar as* diferenças de API do processo para [migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)

Alguns métodos do Azure AD Graph também foram alterados.  Se um  método não for mostrado nesta lista, ele já estará disponível na versão [v1.0](/graph/api/overview) do Microsoft Graph, com exatamente o mesmo nome do Azure AD Graph.

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
