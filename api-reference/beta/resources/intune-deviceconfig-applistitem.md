---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ccf980b0874ea40989eb297abd6bbf455e827f95
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708827"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="85dea-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="85dea-103">appListItem resource type</span></span>

<span data-ttu-id="85dea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85dea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85dea-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="85dea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85dea-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="85dea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85dea-107">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="85dea-107">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="85dea-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85dea-108">Properties</span></span>
|<span data-ttu-id="85dea-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85dea-109">Property</span></span>|<span data-ttu-id="85dea-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="85dea-110">Type</span></span>|<span data-ttu-id="85dea-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="85dea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85dea-112">nome</span><span class="sxs-lookup"><span data-stu-id="85dea-112">name</span></span>|<span data-ttu-id="85dea-113">String</span><span class="sxs-lookup"><span data-stu-id="85dea-113">String</span></span>|<span data-ttu-id="85dea-114">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="85dea-114">The application name</span></span>|
|<span data-ttu-id="85dea-115">distribuidor</span><span class="sxs-lookup"><span data-stu-id="85dea-115">publisher</span></span>|<span data-ttu-id="85dea-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85dea-116">String</span></span>|<span data-ttu-id="85dea-117">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="85dea-117">The publisher of the application</span></span>|
|<span data-ttu-id="85dea-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="85dea-118">appStoreUrl</span></span>|<span data-ttu-id="85dea-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85dea-119">String</span></span>|<span data-ttu-id="85dea-120">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="85dea-120">The Store URL of the application</span></span>|
|<span data-ttu-id="85dea-121">appId</span><span class="sxs-lookup"><span data-stu-id="85dea-121">appId</span></span>|<span data-ttu-id="85dea-122">String</span><span class="sxs-lookup"><span data-stu-id="85dea-122">String</span></span>|<span data-ttu-id="85dea-123">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="85dea-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="85dea-124">Relações</span><span class="sxs-lookup"><span data-stu-id="85dea-124">Relationships</span></span>
<span data-ttu-id="85dea-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="85dea-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85dea-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85dea-126">JSON Representation</span></span>
<span data-ttu-id="85dea-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="85dea-127">Here is a JSON representation of the resource.</span></span>
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





