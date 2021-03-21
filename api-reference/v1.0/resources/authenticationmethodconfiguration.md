---
title: authenticationMethodConfigurations
description: objeto authenticationMethodConfigurations.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 083ace96234a724fc4c9f6e1cdda0cbd8a99e22a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964616"
---
# <a name="authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="f11a7-103">tipo de recurso authenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="f11a7-103">authenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="f11a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f11a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f11a7-105">Representa uma política de método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="f11a7-105">Represents an authentication method policy.</span></span>

## <a name="properties"></a><span data-ttu-id="f11a7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f11a7-106">Properties</span></span>
|<span data-ttu-id="f11a7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f11a7-107">Property</span></span>|<span data-ttu-id="f11a7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f11a7-108">Type</span></span>|<span data-ttu-id="f11a7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f11a7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f11a7-110">id</span><span class="sxs-lookup"><span data-stu-id="f11a7-110">id</span></span>|<span data-ttu-id="f11a7-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f11a7-111">String</span></span>|<span data-ttu-id="f11a7-112">O nome da política.</span><span class="sxs-lookup"><span data-stu-id="f11a7-112">The policy name.</span></span>|
|<span data-ttu-id="f11a7-113">estado</span><span class="sxs-lookup"><span data-stu-id="f11a7-113">state</span></span>|<span data-ttu-id="f11a7-114">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="f11a7-114">authenticationMethodState</span></span>|<span data-ttu-id="f11a7-115">O estado da política.</span><span class="sxs-lookup"><span data-stu-id="f11a7-115">The state of the policy.</span></span> <span data-ttu-id="f11a7-116">Os valores possíveis são: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f11a7-116">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f11a7-117">Relações</span><span class="sxs-lookup"><span data-stu-id="f11a7-117">Relationships</span></span>
<span data-ttu-id="f11a7-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f11a7-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f11a7-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f11a7-119">JSON representation</span></span>
<span data-ttu-id="f11a7-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f11a7-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```
