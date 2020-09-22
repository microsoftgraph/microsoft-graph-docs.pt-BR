---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4d31623ca3bd23c28398c2c04095f21e00c51b4d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075970"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="55793-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="55793-103">appListItem resource type</span></span>

<span data-ttu-id="55793-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55793-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55793-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="55793-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55793-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55793-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55793-107">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="55793-107">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="55793-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55793-108">Properties</span></span>
|<span data-ttu-id="55793-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55793-109">Property</span></span>|<span data-ttu-id="55793-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="55793-110">Type</span></span>|<span data-ttu-id="55793-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="55793-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55793-112">name</span><span class="sxs-lookup"><span data-stu-id="55793-112">name</span></span>|<span data-ttu-id="55793-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55793-113">String</span></span>|<span data-ttu-id="55793-114">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="55793-114">The application name</span></span>|
|<span data-ttu-id="55793-115">distribuidor</span><span class="sxs-lookup"><span data-stu-id="55793-115">publisher</span></span>|<span data-ttu-id="55793-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55793-116">String</span></span>|<span data-ttu-id="55793-117">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="55793-117">The publisher of the application</span></span>|
|<span data-ttu-id="55793-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="55793-118">appStoreUrl</span></span>|<span data-ttu-id="55793-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55793-119">String</span></span>|<span data-ttu-id="55793-120">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="55793-120">The Store URL of the application</span></span>|
|<span data-ttu-id="55793-121">appId</span><span class="sxs-lookup"><span data-stu-id="55793-121">appId</span></span>|<span data-ttu-id="55793-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55793-122">String</span></span>|<span data-ttu-id="55793-123">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="55793-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="55793-124">Relações</span><span class="sxs-lookup"><span data-stu-id="55793-124">Relationships</span></span>
<span data-ttu-id="55793-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55793-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55793-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55793-126">JSON Representation</span></span>
<span data-ttu-id="55793-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55793-127">Here is a JSON representation of the resource.</span></span>
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






