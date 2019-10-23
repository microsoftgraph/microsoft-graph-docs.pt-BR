---
title: tipo de recurso cloudAppSecuritySessionControl
description: Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 105a60905bd69317d152d9609e0a95fb78610a35
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638593"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="a18d9-103">tipo de recurso cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="a18d9-103">cloudAppSecuritySessionControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a18d9-104">Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem.</span><span class="sxs-lookup"><span data-stu-id="a18d9-104">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="a18d9-105">Inehrits do [controle de sessão de acesso condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="a18d9-105">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a18d9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a18d9-106">Properties</span></span>

| <span data-ttu-id="a18d9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a18d9-107">Property</span></span>     | <span data-ttu-id="a18d9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a18d9-108">Type</span></span>        | <span data-ttu-id="a18d9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a18d9-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a18d9-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a18d9-110">isEnabled</span></span>     |<span data-ttu-id="a18d9-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="a18d9-111">Boolean</span></span>      | <span data-ttu-id="a18d9-112">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="a18d9-112">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="a18d9-113">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="a18d9-113">cloudAppSecurityType</span></span>|<span data-ttu-id="a18d9-114">String</span><span class="sxs-lookup"><span data-stu-id="a18d9-114">String</span></span> | <span data-ttu-id="a18d9-115">Os valores possíveis são: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span><span class="sxs-lookup"><span data-stu-id="a18d9-115">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span></span> <span data-ttu-id="a18d9-116">Saiba mais sobre estes valores aqui:https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span><span class="sxs-lookup"><span data-stu-id="a18d9-116">Learn more about these values here: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span></span> |

## <a name="relationships"></a><span data-ttu-id="a18d9-117">Relações</span><span class="sxs-lookup"><span data-stu-id="a18d9-117">Relationships</span></span>

<span data-ttu-id="a18d9-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a18d9-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a18d9-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a18d9-119">JSON representation</span></span>

<span data-ttu-id="a18d9-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a18d9-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecuritySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "cloudAppSecurityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecuritySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->