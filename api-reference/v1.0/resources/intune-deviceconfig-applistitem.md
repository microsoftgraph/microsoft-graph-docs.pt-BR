---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: acb27cacd61685c36043789b25f70f015d1fe0b8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530927"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="7f410-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="7f410-103">appListItem resource type</span></span>

<span data-ttu-id="7f410-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f410-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f410-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f410-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f410-106">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="7f410-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="7f410-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f410-107">Properties</span></span>
|<span data-ttu-id="7f410-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f410-108">Property</span></span>|<span data-ttu-id="7f410-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f410-109">Type</span></span>|<span data-ttu-id="7f410-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f410-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f410-111">nome</span><span class="sxs-lookup"><span data-stu-id="7f410-111">name</span></span>|<span data-ttu-id="7f410-112">String</span><span class="sxs-lookup"><span data-stu-id="7f410-112">String</span></span>|<span data-ttu-id="7f410-113">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f410-113">The application name</span></span>|
|<span data-ttu-id="7f410-114">distribuidor</span><span class="sxs-lookup"><span data-stu-id="7f410-114">publisher</span></span>|<span data-ttu-id="7f410-115">String</span><span class="sxs-lookup"><span data-stu-id="7f410-115">String</span></span>|<span data-ttu-id="7f410-116">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f410-116">The publisher of the application</span></span>|
|<span data-ttu-id="7f410-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7f410-117">appStoreUrl</span></span>|<span data-ttu-id="7f410-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f410-118">String</span></span>|<span data-ttu-id="7f410-119">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f410-119">The Store URL of the application</span></span>|
|<span data-ttu-id="7f410-120">appId</span><span class="sxs-lookup"><span data-stu-id="7f410-120">appId</span></span>|<span data-ttu-id="7f410-121">String</span><span class="sxs-lookup"><span data-stu-id="7f410-121">String</span></span>|<span data-ttu-id="7f410-122">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f410-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f410-123">Relações</span><span class="sxs-lookup"><span data-stu-id="7f410-123">Relationships</span></span>
<span data-ttu-id="7f410-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7f410-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f410-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f410-125">JSON Representation</span></span>
<span data-ttu-id="7f410-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f410-126">Here is a JSON representation of the resource.</span></span>
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




