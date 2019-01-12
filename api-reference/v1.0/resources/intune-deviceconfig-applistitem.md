---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a70f68d291036a7a01823c1946aac655aee6e71c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954425"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="8496c-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="8496c-103">appListItem resource type</span></span>

> <span data-ttu-id="8496c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8496c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8496c-105">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="8496c-105">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="8496c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8496c-106">Properties</span></span>
|<span data-ttu-id="8496c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8496c-107">Property</span></span>|<span data-ttu-id="8496c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8496c-108">Type</span></span>|<span data-ttu-id="8496c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8496c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8496c-110">name</span><span class="sxs-lookup"><span data-stu-id="8496c-110">name</span></span>|<span data-ttu-id="8496c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8496c-111">String</span></span>|<span data-ttu-id="8496c-112">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="8496c-112">The application name</span></span>|
|<span data-ttu-id="8496c-113">distribuidor</span><span class="sxs-lookup"><span data-stu-id="8496c-113">publisher</span></span>|<span data-ttu-id="8496c-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8496c-114">String</span></span>|<span data-ttu-id="8496c-115">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="8496c-115">The publisher of the application</span></span>|
|<span data-ttu-id="8496c-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="8496c-116">appStoreUrl</span></span>|<span data-ttu-id="8496c-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8496c-117">String</span></span>|<span data-ttu-id="8496c-118">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="8496c-118">The Store URL of the application</span></span>|
|<span data-ttu-id="8496c-119">appId</span><span class="sxs-lookup"><span data-stu-id="8496c-119">appId</span></span>|<span data-ttu-id="8496c-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8496c-120">String</span></span>|<span data-ttu-id="8496c-121">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="8496c-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="8496c-122">Relações</span><span class="sxs-lookup"><span data-stu-id="8496c-122">Relationships</span></span>
<span data-ttu-id="8496c-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8496c-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8496c-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8496c-124">JSON Representation</span></span>
<span data-ttu-id="8496c-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8496c-125">Here is a JSON representation of the resource.</span></span>
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



