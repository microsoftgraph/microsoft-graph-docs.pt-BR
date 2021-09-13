---
title: Examinar Azure Active Directory (Azure AD) Graph uso do aplicativo APIs
description: Descreve como auditar Azure Active Directory (Azure AD) Graph APIs para migrar um aplicativo para a API Graph Microsoft.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 8386c3c77a5f42115236875d8405f97c5f49ff42
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139167"
---
# <a name="examine-azure-active-directory-azure-ad-graph-apis-app-usage"></a>Examinar Azure Active Directory (Azure AD) Graph uso do aplicativo APIs

Esta é a etapa 2 do [processo para migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)

Ao planejar sua migração para o Microsoft Graph, leve tempo para revisar seu aplicativo existente e para catalogar as APIs do Azure AD Graph que você está usando no momento.

Compare sua lista com as diferenças conhecidas.  Isso ajuda a identificar alterações específicas que você precisará fazer para migrar seu aplicativo.  Elas incluem alterações simples facilmente resolvidas usando os recursos de pesquisa e substituição de um editor ou atualizações mais complicadas que podem exigir mais análise.

O microsoft Graph oferece suporte a muitos dos mesmos recursos e recursos do gráfico do Azure AD.  Há algumas diferenças importantes:

- [Diferenças de solicitação](migrate-azure-ad-graph-request-differences.md)
- [Diferenças de recursos](migrate-azure-ad-graph-feature-differences.md)
- [Diferenças de tipo de recurso](migrate-azure-ad-graph-resource-differences.md)
- [Diferenças de propriedades](migrate-azure-ad-graph-property-differences.md)
- [Diferenças de método](migrate-azure-ad-graph-method-differences.md)

Você também vai querer verificar as permissões necessárias para os recursos que seu aplicativo está usando.  Em alguns casos, permissões mais granulares estão disponíveis.

Para saber mais, confira [permissões](permissions-reference.md).

## <a name="next-steps"></a>Próximas etapas

- Saiba mais [sobre o registro de aplicativos, permissões](migrate-azure-ad-graph-app-registration.md) e diferenças de consentimento entre o Azure AD Graph e o Microsoft Graph.
- Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.

