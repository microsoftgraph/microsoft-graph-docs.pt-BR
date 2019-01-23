---
title: Tipo de recurso windowsInformationProtectionResourceCollection
description: Coleção de recursos da Proteção de Informações do Windows
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c4a8ad51177507613c3fd84b524503d0e79c208f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424676"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="79de0-103">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="79de0-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="79de0-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="79de0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="79de0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="79de0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79de0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="79de0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79de0-107">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="79de0-107">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="79de0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79de0-108">Properties</span></span>
|<span data-ttu-id="79de0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79de0-109">Property</span></span>|<span data-ttu-id="79de0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="79de0-110">Type</span></span>|<span data-ttu-id="79de0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="79de0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79de0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="79de0-112">displayName</span></span>|<span data-ttu-id="79de0-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79de0-113">String</span></span>|<span data-ttu-id="79de0-114">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="79de0-114">Display name</span></span>|
|<span data-ttu-id="79de0-115">recursos</span><span class="sxs-lookup"><span data-stu-id="79de0-115">resources</span></span>|<span data-ttu-id="79de0-116">String collection</span><span class="sxs-lookup"><span data-stu-id="79de0-116">String collection</span></span>|<span data-ttu-id="79de0-117">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="79de0-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="79de0-118">Relações</span><span class="sxs-lookup"><span data-stu-id="79de0-118">Relationships</span></span>
<span data-ttu-id="79de0-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79de0-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79de0-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79de0-120">JSON Representation</span></span>
<span data-ttu-id="79de0-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79de0-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```




