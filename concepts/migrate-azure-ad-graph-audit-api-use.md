---
title: Examinar o uso do aplicativo APIs do Azure AD Graph
description: Descreve como auditar as APIs do Azure Active Directory (Azure AD) para migrar um aplicativo para a API do Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 405c68d1e0f88af33caa7b5f4c083bd1acdec82d
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872961"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a>Examinar o uso do aplicativo APIs do Azure AD Graph

Esta é a etapa 2 do [processo de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md).

Ao planejar sua migração para o Microsoft Graph, Reserve um tempo para revisar seu aplicativo existente e catalogar as APIs do Azure AD Graph que você está usando no momento.

Compare sua lista com as diferenças conhecidas.  Isso ajuda a identificar alterações específicas que você precisará fazer para migrar seu aplicativo.  Eles incluem alterações simples facilmente resolvidas usando os recursos de pesquisa e substituição de um editor ou atualizações mais complicadas que podem exigir mais análise.

O Microsoft Graph oferece suporte a muitos dos mesmos recursos e funcionalidades do Azure AD Graph.  Há algumas diferenças importantes:

- [Solicitar diferenças](migrate-azure-ad-graph-request-differences.md)
- [Diferenças de recursos](migrate-azure-ad-graph-feature-differences.md)
- [Diferenças de tipo de recurso](migrate-azure-ad-graph-resource-differences.md)
- [Diferenças de propriedade](migrate-azure-ad-graph-property-differences.md)
- [Diferenças de método](migrate-azure-ad-graph-method-differences.md)

Você também deve verificar as permissões necessárias para os recursos que seu aplicativo está usando.  Em alguns casos, as permissões mais granulares estão disponíveis.

Para saber mais, confira [permissões](permissions-reference.md).

## <a name="next-steps"></a>Próximas etapas

- Saiba mais sobre [as diferenças de registro de aplicativo, permissões e consentimento](migrate-azure-ad-graph-app-registration.md) entre o Azure ad Graph e o Microsoft Graph.
- Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.

