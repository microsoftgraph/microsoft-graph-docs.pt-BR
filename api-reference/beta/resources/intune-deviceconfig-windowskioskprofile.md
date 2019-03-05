---
title: tipo de recurso windowsKioskProfile
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1c7107982a33452cd9dd00829cba08f108c6394
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164747"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="f0e46-103">tipo de recurso windowsKioskProfile</span><span class="sxs-lookup"><span data-stu-id="f0e46-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="f0e46-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f0e46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0e46-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0e46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0e46-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f0e46-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f0e46-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0e46-107">Properties</span></span>
|<span data-ttu-id="f0e46-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0e46-108">Property</span></span>|<span data-ttu-id="f0e46-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0e46-109">Type</span></span>|<span data-ttu-id="f0e46-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0e46-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0e46-111">ProfileId</span><span class="sxs-lookup"><span data-stu-id="f0e46-111">profileId</span></span>|<span data-ttu-id="f0e46-112">String</span><span class="sxs-lookup"><span data-stu-id="f0e46-112">String</span></span>|<span data-ttu-id="f0e46-113">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f0e46-113">Key of the entity.</span></span>|
|<span data-ttu-id="f0e46-114">ProfileName</span><span class="sxs-lookup"><span data-stu-id="f0e46-114">profileName</span></span>|<span data-ttu-id="f0e46-115">String</span><span class="sxs-lookup"><span data-stu-id="f0e46-115">String</span></span>|<span data-ttu-id="f0e46-116">Este é um nome amigável usado para identificar um grupo de aplicativos, o layout desses aplicativos no menu iniciar e os usuários aos quais esta configuração de quiosque é atribuída.</span><span class="sxs-lookup"><span data-stu-id="f0e46-116">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="f0e46-117">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="f0e46-117">appConfiguration</span></span>|[<span data-ttu-id="f0e46-118">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="f0e46-118">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="f0e46-119">A configuração do aplicativo que será usada para esta configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="f0e46-119">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="f0e46-120">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="f0e46-120">userAccountsConfiguration</span></span>|<span data-ttu-id="f0e46-121">coleção [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="f0e46-121">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="f0e46-122">As contas de usuário que serão bloqueadas para esta configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="f0e46-122">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="f0e46-123">Essa coleção pode conter um máximo de 100 elementos.</span><span class="sxs-lookup"><span data-stu-id="f0e46-123">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0e46-124">Relações</span><span class="sxs-lookup"><span data-stu-id="f0e46-124">Relationships</span></span>
<span data-ttu-id="f0e46-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0e46-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0e46-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0e46-126">JSON Representation</span></span>
<span data-ttu-id="f0e46-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0e46-127">Here is a JSON representation of the resource.</span></span>
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
        "appType": "String",
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




