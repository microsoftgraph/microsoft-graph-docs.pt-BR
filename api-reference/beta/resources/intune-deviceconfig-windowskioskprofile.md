---
title: tipo de recurso de windowsKioskProfile
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6fc462bdf6548f0f281082ba1cb228796899896d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977049"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="226b4-103">tipo de recurso de windowsKioskProfile</span><span class="sxs-lookup"><span data-stu-id="226b4-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="226b4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="226b4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="226b4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="226b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="226b4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="226b4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="226b4-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="226b4-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="226b4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="226b4-108">Properties</span></span>
|<span data-ttu-id="226b4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="226b4-109">Property</span></span>|<span data-ttu-id="226b4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="226b4-110">Type</span></span>|<span data-ttu-id="226b4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="226b4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="226b4-112">profileId</span><span class="sxs-lookup"><span data-stu-id="226b4-112">profileId</span></span>|<span data-ttu-id="226b4-113">String</span><span class="sxs-lookup"><span data-stu-id="226b4-113">String</span></span>|<span data-ttu-id="226b4-114">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="226b4-114">Key of the entity.</span></span>|
|<span data-ttu-id="226b4-115">profileName</span><span class="sxs-lookup"><span data-stu-id="226b4-115">profileName</span></span>|<span data-ttu-id="226b4-116">String</span><span class="sxs-lookup"><span data-stu-id="226b4-116">String</span></span>|<span data-ttu-id="226b4-117">Este é um nome amigável usado para identificar um grupo de aplicativos, o layout desses aplicativos no menu Iniciar e os usuários aos quais essa configuração de quiosque é atribuída.</span><span class="sxs-lookup"><span data-stu-id="226b4-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="226b4-118">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="226b4-118">appConfiguration</span></span>|[<span data-ttu-id="226b4-119">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="226b4-119">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="226b4-120">A configuração do aplicativo que será usada para esta configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="226b4-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="226b4-121">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="226b4-121">userAccountsConfiguration</span></span>|<span data-ttu-id="226b4-122">coleção [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="226b4-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="226b4-123">As contas de usuário que serão bloqueadas para esta configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="226b4-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="226b4-124">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="226b4-124">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="226b4-125">Relações</span><span class="sxs-lookup"><span data-stu-id="226b4-125">Relationships</span></span>
<span data-ttu-id="226b4-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="226b4-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="226b4-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="226b4-127">JSON Representation</span></span>
<span data-ttu-id="226b4-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="226b4-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskProfile",
  "profileId": "String",
  "profileName": "String",
  "appConfiguration": {
    "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
    "apps": [
      {
        "@odata.type": "microsoft.graph.windowsKioskUWPApp",
        "startLayoutTileSize": "String",
        "name": "String",
        "appUserModelId": "String",
        "appId": "String",
        "containedAppId": "String"
      }
    ],
    "showTaskBar": true,
    "disallowDesktopApps": true,
    "startMenuLayoutXml": "binary"
  },
  "userAccountsConfiguration": [
    {
      "@odata.type": "microsoft.graph.windowsKioskVisitor"
    }
  ]
}
```





