---
title: tipo de recurso microsoftStoreForBusinessAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8ef23919912d8a91beceefeb034de7cc09cb941c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805019"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="1f648-103">tipo de recurso microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="1f648-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="1f648-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1f648-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f648-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1f648-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f648-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1f648-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f648-107">Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.</span><span class="sxs-lookup"><span data-stu-id="1f648-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="1f648-108">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="1f648-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1f648-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f648-109">Properties</span></span>
|<span data-ttu-id="1f648-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f648-110">Property</span></span>|<span data-ttu-id="1f648-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f648-111">Type</span></span>|<span data-ttu-id="1f648-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f648-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f648-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="1f648-113">useDeviceContext</span></span>|<span data-ttu-id="1f648-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="1f648-114">Boolean</span></span>|<span data-ttu-id="1f648-115">Se é para usar ou não o contexto de execução do dispositivo em aplicativo móvel da Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="1f648-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f648-116">Relações</span><span class="sxs-lookup"><span data-stu-id="1f648-116">Relationships</span></span>
<span data-ttu-id="1f648-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f648-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1f648-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f648-118">JSON Representation</span></span>
<span data-ttu-id="1f648-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f648-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```





