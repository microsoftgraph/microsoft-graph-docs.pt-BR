---
title: tipo de recurso windowsKioskProfile
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 48d20c46c305ee4c6f9bec99ba2c531bab1aa83e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464078"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="0da4e-103">tipo de recurso windowsKioskProfile</span><span class="sxs-lookup"><span data-stu-id="0da4e-103">windowsKioskProfile resource type</span></span>

<span data-ttu-id="0da4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0da4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0da4e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0da4e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0da4e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0da4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0da4e-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0da4e-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0da4e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0da4e-108">Properties</span></span>
|<span data-ttu-id="0da4e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0da4e-109">Property</span></span>|<span data-ttu-id="0da4e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0da4e-110">Type</span></span>|<span data-ttu-id="0da4e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0da4e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0da4e-112">ProfileId</span><span class="sxs-lookup"><span data-stu-id="0da4e-112">profileId</span></span>|<span data-ttu-id="0da4e-113">String</span><span class="sxs-lookup"><span data-stu-id="0da4e-113">String</span></span>|<span data-ttu-id="0da4e-114">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0da4e-114">Key of the entity.</span></span>|
|<span data-ttu-id="0da4e-115">ProfileName</span><span class="sxs-lookup"><span data-stu-id="0da4e-115">profileName</span></span>|<span data-ttu-id="0da4e-116">String</span><span class="sxs-lookup"><span data-stu-id="0da4e-116">String</span></span>|<span data-ttu-id="0da4e-117">Este é um nome amigável usado para identificar um grupo de aplicativos, o layout desses aplicativos no menu iniciar e os usuários aos quais esta configuração de quiosque é atribuída.</span><span class="sxs-lookup"><span data-stu-id="0da4e-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="0da4e-118">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="0da4e-118">appConfiguration</span></span>|[<span data-ttu-id="0da4e-119">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="0da4e-119">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="0da4e-120">A configuração do aplicativo que será usada para esta configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="0da4e-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="0da4e-121">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="0da4e-121">userAccountsConfiguration</span></span>|<span data-ttu-id="0da4e-122">coleção [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="0da4e-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="0da4e-123">As contas de usuário que serão bloqueadas para esta configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="0da4e-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="0da4e-124">Essa coleção pode conter um máximo de 100 elementos.</span><span class="sxs-lookup"><span data-stu-id="0da4e-124">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0da4e-125">Relações</span><span class="sxs-lookup"><span data-stu-id="0da4e-125">Relationships</span></span>
<span data-ttu-id="0da4e-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0da4e-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0da4e-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0da4e-127">JSON Representation</span></span>
<span data-ttu-id="0da4e-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0da4e-128">Here is a JSON representation of the resource.</span></span>
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
        "autoLaunch": true,
        "appUserModelId": "String",
        "appId": "String",
        "containedAppId": "String"
      }
    ],
    "showTaskBar": true,
    "allowAccessToDownloadsFolder": true,
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



