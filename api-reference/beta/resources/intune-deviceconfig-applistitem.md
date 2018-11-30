---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
ms.openlocfilehash: 16d191bb53f7546598b7869e8bc28be07cc4f604
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037557"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="1b22c-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="1b22c-103">appListItem resource type</span></span>

> <span data-ttu-id="1b22c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1b22c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b22c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1b22c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b22c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1b22c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b22c-107">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="1b22c-107">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="1b22c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b22c-108">Properties</span></span>
|<span data-ttu-id="1b22c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b22c-109">Property</span></span>|<span data-ttu-id="1b22c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b22c-110">Type</span></span>|<span data-ttu-id="1b22c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b22c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b22c-112">name</span><span class="sxs-lookup"><span data-stu-id="1b22c-112">name</span></span>|<span data-ttu-id="1b22c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b22c-113">String</span></span>|<span data-ttu-id="1b22c-114">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b22c-114">The application name</span></span>|
|<span data-ttu-id="1b22c-115">distribuidor</span><span class="sxs-lookup"><span data-stu-id="1b22c-115">publisher</span></span>|<span data-ttu-id="1b22c-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b22c-116">String</span></span>|<span data-ttu-id="1b22c-117">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b22c-117">The publisher of the application</span></span>|
|<span data-ttu-id="1b22c-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1b22c-118">appStoreUrl</span></span>|<span data-ttu-id="1b22c-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b22c-119">String</span></span>|<span data-ttu-id="1b22c-120">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b22c-120">The Store URL of the application</span></span>|
|<span data-ttu-id="1b22c-121">appId</span><span class="sxs-lookup"><span data-stu-id="1b22c-121">appId</span></span>|<span data-ttu-id="1b22c-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b22c-122">String</span></span>|<span data-ttu-id="1b22c-123">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b22c-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b22c-124">Relações</span><span class="sxs-lookup"><span data-stu-id="1b22c-124">Relationships</span></span>
<span data-ttu-id="1b22c-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b22c-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1b22c-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b22c-126">JSON Representation</span></span>
<span data-ttu-id="1b22c-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b22c-127">Here is a JSON representation of the resource.</span></span>
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





