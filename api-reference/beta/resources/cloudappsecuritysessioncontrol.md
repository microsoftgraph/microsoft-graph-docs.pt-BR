---
title: tipo de recurso cloudAppSecuritySessionControl
description: Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4665fc3456dbd6375ea0ef9651455427e74b732f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034067"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="2c15d-103">tipo de recurso cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="2c15d-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="2c15d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c15d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c15d-105">Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem.</span><span class="sxs-lookup"><span data-stu-id="2c15d-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="2c15d-106">Inehrits do [controle de sessão de acesso condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="2c15d-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2c15d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c15d-107">Properties</span></span>

| <span data-ttu-id="2c15d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c15d-108">Property</span></span>     | <span data-ttu-id="2c15d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c15d-109">Type</span></span>        | <span data-ttu-id="2c15d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c15d-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2c15d-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="2c15d-111">isEnabled</span></span>     |<span data-ttu-id="2c15d-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c15d-112">Boolean</span></span>      | <span data-ttu-id="2c15d-113">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="2c15d-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="2c15d-114">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="2c15d-114">cloudAppSecurityType</span></span>|<span data-ttu-id="2c15d-115">String</span><span class="sxs-lookup"><span data-stu-id="2c15d-115">String</span></span> | <span data-ttu-id="2c15d-116">Os valores possíveis são: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span><span class="sxs-lookup"><span data-stu-id="2c15d-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span></span> <span data-ttu-id="2c15d-117">Saiba mais sobre estes valores aqui: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span><span class="sxs-lookup"><span data-stu-id="2c15d-117">Learn more about these values here: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span></span> |

## <a name="relationships"></a><span data-ttu-id="2c15d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="2c15d-118">Relationships</span></span>

<span data-ttu-id="2c15d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c15d-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c15d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c15d-120">JSON representation</span></span>

<span data-ttu-id="2c15d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c15d-121">The following is a JSON representation of the resource.</span></span>

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

