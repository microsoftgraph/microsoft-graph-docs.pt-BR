---
title: tipo de recurso cloudAppSecuritySessionControl
description: Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 114e788e12ab8f633bc6350b08140f9d5e4fe8a3
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581264"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="50cf8-103">tipo de recurso cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="50cf8-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="50cf8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50cf8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="50cf8-105">Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem.</span><span class="sxs-lookup"><span data-stu-id="50cf8-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="50cf8-106">Inehrits do [controle de sessão de acesso condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="50cf8-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="50cf8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50cf8-107">Properties</span></span>

| <span data-ttu-id="50cf8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50cf8-108">Property</span></span>     | <span data-ttu-id="50cf8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="50cf8-109">Type</span></span>        | <span data-ttu-id="50cf8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="50cf8-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="50cf8-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="50cf8-111">isEnabled</span></span>     |<span data-ttu-id="50cf8-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="50cf8-112">Boolean</span></span>      | <span data-ttu-id="50cf8-113">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="50cf8-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="50cf8-114">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="50cf8-114">cloudAppSecurityType</span></span>|<span data-ttu-id="50cf8-115">String</span><span class="sxs-lookup"><span data-stu-id="50cf8-115">String</span></span>| <span data-ttu-id="50cf8-116">Os valores possíveis são: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="50cf8-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span></span> <span data-ttu-id="50cf8-117">Para obter mais informações, consulte [Deploy Conditional Access app Control for refeatured apps](/cloud-app-security/proxy-deployment-aad).</span><span class="sxs-lookup"><span data-stu-id="50cf8-117">For more information, see [Deploy Conditional Access App Control for featured apps](/cloud-app-security/proxy-deployment-aad).</span></span> |

## <a name="relationships"></a><span data-ttu-id="50cf8-118">Relações</span><span class="sxs-lookup"><span data-stu-id="50cf8-118">Relationships</span></span>

<span data-ttu-id="50cf8-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50cf8-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="50cf8-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50cf8-120">JSON representation</span></span>

<span data-ttu-id="50cf8-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50cf8-121">The following is a JSON representation of the resource.</span></span>

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