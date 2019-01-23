---
title: tipo de recurso de macOSLobChildApp
description: Contém propriedades o MacOS LOB App em um pacote de pacote
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a6a8cafc0f9b47f40fe7e922130a41d37a427e5e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403018"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="24765-103">tipo de recurso de macOSLobChildApp</span><span class="sxs-lookup"><span data-stu-id="24765-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="24765-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="24765-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="24765-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="24765-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24765-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="24765-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24765-107">Contém propriedades o MacOS LOB App em um pacote de pacote</span><span class="sxs-lookup"><span data-stu-id="24765-107">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="24765-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="24765-108">Properties</span></span>
|<span data-ttu-id="24765-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24765-109">Property</span></span>|<span data-ttu-id="24765-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="24765-110">Type</span></span>|<span data-ttu-id="24765-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="24765-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24765-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="24765-112">bundleId</span></span>|<span data-ttu-id="24765-113">String</span><span class="sxs-lookup"><span data-stu-id="24765-113">String</span></span>|<span data-ttu-id="24765-114">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="24765-114">The Identity Name.</span></span>|
|<span data-ttu-id="24765-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="24765-115">buildNumber</span></span>|<span data-ttu-id="24765-116">String</span><span class="sxs-lookup"><span data-stu-id="24765-116">String</span></span>|<span data-ttu-id="24765-117">O número de compilação da linha de MacOS do aplicativo de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="24765-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="24765-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="24765-118">versionNumber</span></span>|<span data-ttu-id="24765-119">String</span><span class="sxs-lookup"><span data-stu-id="24765-119">String</span></span>|<span data-ttu-id="24765-120">O número de versão da linha de MacOS do aplicativo de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="24765-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24765-121">Relações</span><span class="sxs-lookup"><span data-stu-id="24765-121">Relationships</span></span>
<span data-ttu-id="24765-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="24765-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24765-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="24765-123">JSON Representation</span></span>
<span data-ttu-id="24765-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="24765-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```




