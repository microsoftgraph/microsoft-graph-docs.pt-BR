---
title: tipo de recurso windowsKioskProfile
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c69c8d32be23dccc935d1de74b0a450850091722
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268213"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="1575c-103">tipo de recurso windowsKioskProfile</span><span class="sxs-lookup"><span data-stu-id="1575c-103">windowsKioskProfile resource type</span></span>

<span data-ttu-id="1575c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1575c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1575c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1575c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1575c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1575c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1575c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1575c-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1575c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1575c-108">Properties</span></span>
|<span data-ttu-id="1575c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1575c-109">Property</span></span>|<span data-ttu-id="1575c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1575c-110">Type</span></span>|<span data-ttu-id="1575c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1575c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1575c-112">ProfileId</span><span class="sxs-lookup"><span data-stu-id="1575c-112">profileId</span></span>|<span data-ttu-id="1575c-113">String</span><span class="sxs-lookup"><span data-stu-id="1575c-113">String</span></span>|<span data-ttu-id="1575c-114">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1575c-114">Key of the entity.</span></span>|
|<span data-ttu-id="1575c-115">ProfileName</span><span class="sxs-lookup"><span data-stu-id="1575c-115">profileName</span></span>|<span data-ttu-id="1575c-116">String</span><span class="sxs-lookup"><span data-stu-id="1575c-116">String</span></span>|<span data-ttu-id="1575c-117">Este é um nome amigável usado para identificar um grupo de aplicativos, o layout desses aplicativos no menu iniciar e os usuários aos quais esta configuração de quiosque é atribuída.</span><span class="sxs-lookup"><span data-stu-id="1575c-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="1575c-118">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="1575c-118">appConfiguration</span></span>|[<span data-ttu-id="1575c-119">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1575c-119">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="1575c-120">A configuração do aplicativo que será usada para esta configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="1575c-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="1575c-121">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="1575c-121">userAccountsConfiguration</span></span>|<span data-ttu-id="1575c-122">coleção [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="1575c-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="1575c-123">As contas de usuário que serão bloqueadas para esta configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="1575c-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="1575c-124">Essa coleção pode conter um máximo de 100 elementos.</span><span class="sxs-lookup"><span data-stu-id="1575c-124">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1575c-125">Relações</span><span class="sxs-lookup"><span data-stu-id="1575c-125">Relationships</span></span>
<span data-ttu-id="1575c-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1575c-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1575c-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1575c-127">JSON Representation</span></span>
<span data-ttu-id="1575c-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1575c-128">Here is a JSON representation of the resource.</span></span>
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




