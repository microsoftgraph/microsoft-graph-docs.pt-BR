---
title: tipo de recurso de win32LobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel Win32 LOB a um grupo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 215b5c7086c2336f80bc0b812a108fbe2e2c1740
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429079"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="39f6b-103">tipo de recurso de win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="39f6b-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="39f6b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="39f6b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="39f6b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="39f6b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39f6b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="39f6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39f6b-107">Contém propriedades usadas para atribuir um aplicativo móvel Win32 LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="39f6b-107">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="39f6b-108">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="39f6b-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="39f6b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="39f6b-109">Properties</span></span>
|<span data-ttu-id="39f6b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39f6b-110">Property</span></span>|<span data-ttu-id="39f6b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="39f6b-111">Type</span></span>|<span data-ttu-id="39f6b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="39f6b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39f6b-113">notificações</span><span class="sxs-lookup"><span data-stu-id="39f6b-113">notifications</span></span>|[<span data-ttu-id="39f6b-114">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="39f6b-114">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="39f6b-115">O status de notificação essa atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39f6b-115">The notification status this app assignment.</span></span> <span data-ttu-id="39f6b-116">Os valores possíveis são: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="39f6b-116">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39f6b-117">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="39f6b-117">Relationships</span></span>
<span data-ttu-id="39f6b-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="39f6b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="39f6b-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="39f6b-119">JSON Representation</span></span>
<span data-ttu-id="39f6b-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="39f6b-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppAssignmentSettings",
  "notifications": "String"
}
```




