---
title: Tipo de recurso resourceAction
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5442ed8ee55005b1261da09d999e9c27053276d2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415261"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="3cfbe-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="3cfbe-103">resourceAction resource type</span></span>

> <span data-ttu-id="3cfbe-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="3cfbe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3cfbe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3cfbe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3cfbe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="3cfbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cfbe-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3cfbe-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3cfbe-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3cfbe-108">Properties</span></span>
|<span data-ttu-id="3cfbe-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3cfbe-109">Property</span></span>|<span data-ttu-id="3cfbe-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cfbe-110">Type</span></span>|<span data-ttu-id="3cfbe-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cfbe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cfbe-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="3cfbe-112">allowedResourceActions</span></span>|<span data-ttu-id="3cfbe-113">String collection</span><span class="sxs-lookup"><span data-stu-id="3cfbe-113">String collection</span></span>|<span data-ttu-id="3cfbe-114">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="3cfbe-114">Allowed Actions</span></span>|
|<span data-ttu-id="3cfbe-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="3cfbe-115">notAllowedResourceActions</span></span>|<span data-ttu-id="3cfbe-116">String collection</span><span class="sxs-lookup"><span data-stu-id="3cfbe-116">String collection</span></span>|<span data-ttu-id="3cfbe-117">Ações não permitidas</span><span class="sxs-lookup"><span data-stu-id="3cfbe-117">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cfbe-118">Relações</span><span class="sxs-lookup"><span data-stu-id="3cfbe-118">Relationships</span></span>
<span data-ttu-id="3cfbe-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3cfbe-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3cfbe-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3cfbe-120">JSON Representation</span></span>
<span data-ttu-id="3cfbe-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3cfbe-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```




