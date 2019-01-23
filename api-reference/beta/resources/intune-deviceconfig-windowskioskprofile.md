---
title: tipo de recurso de windowsKioskProfile
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55d8c23d3bfae2baf9d632c33390b8aafb5e7ef8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420245"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="c869b-103">tipo de recurso de windowsKioskProfile</span><span class="sxs-lookup"><span data-stu-id="c869b-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="c869b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c869b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c869b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c869b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c869b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c869b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c869b-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c869b-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c869b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c869b-108">Properties</span></span>
|<span data-ttu-id="c869b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c869b-109">Property</span></span>|<span data-ttu-id="c869b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c869b-110">Type</span></span>|<span data-ttu-id="c869b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c869b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c869b-112">profileId</span><span class="sxs-lookup"><span data-stu-id="c869b-112">profileId</span></span>|<span data-ttu-id="c869b-113">String</span><span class="sxs-lookup"><span data-stu-id="c869b-113">String</span></span>|<span data-ttu-id="c869b-114">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c869b-114">Key of the entity.</span></span>|
|<span data-ttu-id="c869b-115">profileName</span><span class="sxs-lookup"><span data-stu-id="c869b-115">profileName</span></span>|<span data-ttu-id="c869b-116">String</span><span class="sxs-lookup"><span data-stu-id="c869b-116">String</span></span>|<span data-ttu-id="c869b-117">Este é um nome amigável usado para identificar um grupo de aplicativos, o layout desses aplicativos no menu Iniciar e os usuários aos quais essa configuração de quiosque é atribuída.</span><span class="sxs-lookup"><span data-stu-id="c869b-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="c869b-118">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="c869b-118">appConfiguration</span></span>|[<span data-ttu-id="c869b-119">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c869b-119">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="c869b-120">A configuração do aplicativo que será usada para esta configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="c869b-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="c869b-121">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="c869b-121">userAccountsConfiguration</span></span>|<span data-ttu-id="c869b-122">coleção [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="c869b-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="c869b-123">As contas de usuário que serão bloqueadas para esta configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="c869b-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="c869b-124">Essa coleção pode conter um máximo de 100 elementos.</span><span class="sxs-lookup"><span data-stu-id="c869b-124">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c869b-125">Relações</span><span class="sxs-lookup"><span data-stu-id="c869b-125">Relationships</span></span>
<span data-ttu-id="c869b-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c869b-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c869b-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c869b-127">JSON Representation</span></span>
<span data-ttu-id="c869b-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c869b-128">Here is a JSON representation of the resource.</span></span>
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




