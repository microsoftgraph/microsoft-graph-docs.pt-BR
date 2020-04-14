---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4a34b8dcfbf3912d5b2a816ddfce6af49596b869
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469956"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="c2fc0-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="c2fc0-103">appListItem resource type</span></span>

<span data-ttu-id="c2fc0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2fc0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2fc0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c2fc0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2fc0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c2fc0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2fc0-107">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="c2fc0-107">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="c2fc0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2fc0-108">Properties</span></span>
|<span data-ttu-id="c2fc0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2fc0-109">Property</span></span>|<span data-ttu-id="c2fc0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2fc0-110">Type</span></span>|<span data-ttu-id="c2fc0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2fc0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2fc0-112">nome</span><span class="sxs-lookup"><span data-stu-id="c2fc0-112">name</span></span>|<span data-ttu-id="c2fc0-113">String</span><span class="sxs-lookup"><span data-stu-id="c2fc0-113">String</span></span>|<span data-ttu-id="c2fc0-114">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2fc0-114">The application name</span></span>|
|<span data-ttu-id="c2fc0-115">distribuidor</span><span class="sxs-lookup"><span data-stu-id="c2fc0-115">publisher</span></span>|<span data-ttu-id="c2fc0-116">String</span><span class="sxs-lookup"><span data-stu-id="c2fc0-116">String</span></span>|<span data-ttu-id="c2fc0-117">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2fc0-117">The publisher of the application</span></span>|
|<span data-ttu-id="c2fc0-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c2fc0-118">appStoreUrl</span></span>|<span data-ttu-id="c2fc0-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2fc0-119">String</span></span>|<span data-ttu-id="c2fc0-120">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2fc0-120">The Store URL of the application</span></span>|
|<span data-ttu-id="c2fc0-121">appId</span><span class="sxs-lookup"><span data-stu-id="c2fc0-121">appId</span></span>|<span data-ttu-id="c2fc0-122">String</span><span class="sxs-lookup"><span data-stu-id="c2fc0-122">String</span></span>|<span data-ttu-id="c2fc0-123">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2fc0-123">The bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2fc0-124">Relações</span><span class="sxs-lookup"><span data-stu-id="c2fc0-124">Relationships</span></span>
<span data-ttu-id="c2fc0-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c2fc0-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2fc0-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c2fc0-126">JSON Representation</span></span>
<span data-ttu-id="c2fc0-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c2fc0-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



