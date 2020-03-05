---
title: tipo de recurso cloudAppSecuritySessionControl
description: Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 35f031498fb3a2f4f9c3a48d0102d57081b7c4d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507646"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="66744-103">tipo de recurso cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="66744-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="66744-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="66744-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66744-105">Controle de sessão usado para impor verificações de segurança do aplicativo na nuvem.</span><span class="sxs-lookup"><span data-stu-id="66744-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="66744-106">Inehrits do [controle de sessão de acesso condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="66744-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="66744-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66744-107">Properties</span></span>

| <span data-ttu-id="66744-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66744-108">Property</span></span>     | <span data-ttu-id="66744-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="66744-109">Type</span></span>        | <span data-ttu-id="66744-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="66744-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="66744-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="66744-111">isEnabled</span></span>     |<span data-ttu-id="66744-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="66744-112">Boolean</span></span>      | <span data-ttu-id="66744-113">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="66744-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="66744-114">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="66744-114">cloudAppSecurityType</span></span>|<span data-ttu-id="66744-115">String</span><span class="sxs-lookup"><span data-stu-id="66744-115">String</span></span> | <span data-ttu-id="66744-116">Os valores possíveis são: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span><span class="sxs-lookup"><span data-stu-id="66744-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span></span> <span data-ttu-id="66744-117">Saiba mais sobre estes valores aqui:https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span><span class="sxs-lookup"><span data-stu-id="66744-117">Learn more about these values here: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span></span> |

## <a name="relationships"></a><span data-ttu-id="66744-118">Relações</span><span class="sxs-lookup"><span data-stu-id="66744-118">Relationships</span></span>

<span data-ttu-id="66744-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66744-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="66744-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66744-120">JSON representation</span></span>

<span data-ttu-id="66744-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66744-121">The following is a JSON representation of the resource.</span></span>

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