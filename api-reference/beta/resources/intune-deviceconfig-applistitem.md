---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: tfitzmac
ms.openlocfilehash: 825e88dd5bd32cadfd9a8bfa291ab67036c8180b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343223"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="43f59-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="43f59-103">appListItem resource type</span></span>

> <span data-ttu-id="43f59-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="43f59-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43f59-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="43f59-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43f59-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="43f59-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43f59-107">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="43f59-107">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="43f59-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43f59-108">Properties</span></span>
|<span data-ttu-id="43f59-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43f59-109">Property</span></span>|<span data-ttu-id="43f59-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="43f59-110">Type</span></span>|<span data-ttu-id="43f59-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="43f59-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43f59-112">name</span><span class="sxs-lookup"><span data-stu-id="43f59-112">name</span></span>|<span data-ttu-id="43f59-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43f59-113">String</span></span>|<span data-ttu-id="43f59-114">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="43f59-114">The application name</span></span>|
|<span data-ttu-id="43f59-115">distribuidor</span><span class="sxs-lookup"><span data-stu-id="43f59-115">publisher</span></span>|<span data-ttu-id="43f59-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43f59-116">String</span></span>|<span data-ttu-id="43f59-117">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="43f59-117">The publisher of the application</span></span>|
|<span data-ttu-id="43f59-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="43f59-118">appStoreUrl</span></span>|<span data-ttu-id="43f59-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43f59-119">String</span></span>|<span data-ttu-id="43f59-120">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="43f59-120">The Store URL of the application</span></span>|
|<span data-ttu-id="43f59-121">appId</span><span class="sxs-lookup"><span data-stu-id="43f59-121">appId</span></span>|<span data-ttu-id="43f59-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43f59-122">String</span></span>|<span data-ttu-id="43f59-123">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="43f59-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="43f59-124">Relações</span><span class="sxs-lookup"><span data-stu-id="43f59-124">Relationships</span></span>
<span data-ttu-id="43f59-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="43f59-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="43f59-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43f59-126">JSON Representation</span></span>
<span data-ttu-id="43f59-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43f59-127">Here is a JSON representation of the resource.</span></span>
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





