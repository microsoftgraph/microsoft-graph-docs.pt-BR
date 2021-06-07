---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0c0e880b8afebdfccab426fbe80966cc3f828a19
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755921"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="69a00-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="69a00-103">appListItem resource type</span></span>

<span data-ttu-id="69a00-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69a00-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69a00-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69a00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69a00-106">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="69a00-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="69a00-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69a00-107">Properties</span></span>
|<span data-ttu-id="69a00-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69a00-108">Property</span></span>|<span data-ttu-id="69a00-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="69a00-109">Type</span></span>|<span data-ttu-id="69a00-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="69a00-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69a00-111">nome</span><span class="sxs-lookup"><span data-stu-id="69a00-111">name</span></span>|<span data-ttu-id="69a00-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69a00-112">String</span></span>|<span data-ttu-id="69a00-113">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="69a00-113">The application name</span></span>|
|<span data-ttu-id="69a00-114">distribuidor</span><span class="sxs-lookup"><span data-stu-id="69a00-114">publisher</span></span>|<span data-ttu-id="69a00-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69a00-115">String</span></span>|<span data-ttu-id="69a00-116">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="69a00-116">The publisher of the application</span></span>|
|<span data-ttu-id="69a00-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="69a00-117">appStoreUrl</span></span>|<span data-ttu-id="69a00-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69a00-118">String</span></span>|<span data-ttu-id="69a00-119">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="69a00-119">The Store URL of the application</span></span>|
|<span data-ttu-id="69a00-120">appId</span><span class="sxs-lookup"><span data-stu-id="69a00-120">appId</span></span>|<span data-ttu-id="69a00-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69a00-121">String</span></span>|<span data-ttu-id="69a00-122">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="69a00-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="69a00-123">Relações</span><span class="sxs-lookup"><span data-stu-id="69a00-123">Relationships</span></span>
<span data-ttu-id="69a00-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="69a00-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69a00-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69a00-125">JSON Representation</span></span>
<span data-ttu-id="69a00-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69a00-126">Here is a JSON representation of the resource.</span></span>
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




