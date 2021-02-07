---
title: Tipo de recurso cloudAppSecuritySessionControl
description: Controle de sessão usado para impor verificações de segurança de aplicativos na nuvem.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b1eee93b3f80b6d7d916f38d783ca94cef8e81a1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133053"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="5f576-103">Tipo de recurso cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="5f576-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="5f576-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f576-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f576-105">Controle de sessão usado para impor verificações de segurança de aplicativos na nuvem.</span><span class="sxs-lookup"><span data-stu-id="5f576-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="5f576-106">Inehrits do [Controle de Sessão de Acesso Condicional.](conditionalaccesssessioncontrol.md)</span><span class="sxs-lookup"><span data-stu-id="5f576-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5f576-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f576-107">Properties</span></span>

| <span data-ttu-id="5f576-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f576-108">Property</span></span>     | <span data-ttu-id="5f576-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f576-109">Type</span></span>        | <span data-ttu-id="5f576-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f576-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5f576-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="5f576-111">isEnabled</span></span>     |<span data-ttu-id="5f576-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="5f576-112">Boolean</span></span>      | <span data-ttu-id="5f576-113">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="5f576-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="5f576-114">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="5f576-114">cloudAppSecurityType</span></span>|<span data-ttu-id="5f576-115">String</span><span class="sxs-lookup"><span data-stu-id="5f576-115">String</span></span>| <span data-ttu-id="5f576-116">Os valores possíveis são: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5f576-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span></span> <span data-ttu-id="5f576-117">Para obter mais informações, [consulte Implantar o Controle de Aplicativo de Acesso Condicional para aplicativos em destaque.](/cloud-app-security/proxy-deployment-aad)</span><span class="sxs-lookup"><span data-stu-id="5f576-117">For more information, see [Deploy Conditional Access App Control for featured apps](/cloud-app-security/proxy-deployment-aad).</span></span> |

## <a name="relationships"></a><span data-ttu-id="5f576-118">Relações</span><span class="sxs-lookup"><span data-stu-id="5f576-118">Relationships</span></span>

<span data-ttu-id="5f576-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f576-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f576-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f576-120">JSON representation</span></span>

<span data-ttu-id="5f576-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f576-121">The following is a JSON representation of the resource.</span></span>

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
