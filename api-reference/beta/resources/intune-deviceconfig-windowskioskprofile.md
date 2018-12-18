---
title: tipo de recurso de windowsKioskProfile
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: ce57b18e86f40a46053a5e0a0f41652763a6d055
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345350"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="ee107-103">tipo de recurso de windowsKioskProfile</span><span class="sxs-lookup"><span data-stu-id="ee107-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="ee107-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ee107-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee107-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ee107-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee107-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ee107-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee107-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ee107-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ee107-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee107-108">Properties</span></span>
|<span data-ttu-id="ee107-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee107-109">Property</span></span>|<span data-ttu-id="ee107-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee107-110">Type</span></span>|<span data-ttu-id="ee107-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee107-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee107-112">profileId</span><span class="sxs-lookup"><span data-stu-id="ee107-112">profileId</span></span>|<span data-ttu-id="ee107-113">String</span><span class="sxs-lookup"><span data-stu-id="ee107-113">String</span></span>|<span data-ttu-id="ee107-114">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ee107-114">Key of the entity.</span></span>|
|<span data-ttu-id="ee107-115">profileName</span><span class="sxs-lookup"><span data-stu-id="ee107-115">profileName</span></span>|<span data-ttu-id="ee107-116">String</span><span class="sxs-lookup"><span data-stu-id="ee107-116">String</span></span>|<span data-ttu-id="ee107-117">Este é um nome amigável usado para identificar um grupo de aplicativos, o layout desses aplicativos no menu Iniciar e os usuários aos quais essa configuração de quiosque é atribuída.</span><span class="sxs-lookup"><span data-stu-id="ee107-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="ee107-118">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee107-118">appConfiguration</span></span>|[<span data-ttu-id="ee107-119">windowsKioskAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee107-119">windowsKioskAppConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|<span data-ttu-id="ee107-120">A configuração do aplicativo que será usada para esta configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="ee107-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="ee107-121">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee107-121">userAccountsConfiguration</span></span>|<span data-ttu-id="ee107-122">coleção [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="ee107-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="ee107-123">As contas de usuário que serão bloqueadas para esta configuração de quiosque.</span><span class="sxs-lookup"><span data-stu-id="ee107-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="ee107-124">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ee107-124">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee107-125">Relações</span><span class="sxs-lookup"><span data-stu-id="ee107-125">Relationships</span></span>
<span data-ttu-id="ee107-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee107-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ee107-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee107-127">JSON Representation</span></span>
<span data-ttu-id="ee107-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee107-128">Here is a JSON representation of the resource.</span></span>
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





