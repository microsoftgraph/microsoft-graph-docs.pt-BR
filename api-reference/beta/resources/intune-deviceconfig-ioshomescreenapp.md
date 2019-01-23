---
title: Tipo de recurso iosHomeScreenApp
description: Representa um ícone de um aplicativo na tela inicial
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dcc90e774f8d032d46968fc4f751923bcc52e559
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412321"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="e3e09-103">Tipo de recurso iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="e3e09-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="e3e09-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e3e09-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e3e09-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e3e09-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3e09-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e3e09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3e09-107">Representa um ícone de um aplicativo na tela inicial</span><span class="sxs-lookup"><span data-stu-id="e3e09-107">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="e3e09-108">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="e3e09-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e3e09-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3e09-109">Properties</span></span>
|<span data-ttu-id="e3e09-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3e09-110">Property</span></span>|<span data-ttu-id="e3e09-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3e09-111">Type</span></span>|<span data-ttu-id="e3e09-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3e09-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3e09-113">displayName</span><span class="sxs-lookup"><span data-stu-id="e3e09-113">displayName</span></span>|<span data-ttu-id="e3e09-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3e09-114">String</span></span>|<span data-ttu-id="e3e09-115">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="e3e09-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="e3e09-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="e3e09-116">bundleID</span></span>|<span data-ttu-id="e3e09-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3e09-117">String</span></span>|<span data-ttu-id="e3e09-118">BundleID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3e09-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3e09-119">Relações</span><span class="sxs-lookup"><span data-stu-id="e3e09-119">Relationships</span></span>
<span data-ttu-id="e3e09-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3e09-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3e09-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3e09-121">JSON Representation</span></span>
<span data-ttu-id="e3e09-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3e09-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```




