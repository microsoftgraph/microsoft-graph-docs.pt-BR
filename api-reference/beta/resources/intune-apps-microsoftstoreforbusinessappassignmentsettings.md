---
title: tipo de recurso microsoftStoreForBusinessAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.
ms.openlocfilehash: 53dc4e9887147253047df67db865c45488b51009
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035172"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="9de97-103">tipo de recurso microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="9de97-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="9de97-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9de97-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9de97-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9de97-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9de97-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9de97-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9de97-107">Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.</span><span class="sxs-lookup"><span data-stu-id="9de97-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="9de97-108">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="9de97-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9de97-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9de97-109">Properties</span></span>
|<span data-ttu-id="9de97-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9de97-110">Property</span></span>|<span data-ttu-id="9de97-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9de97-111">Type</span></span>|<span data-ttu-id="9de97-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9de97-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9de97-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="9de97-113">useDeviceContext</span></span>|<span data-ttu-id="9de97-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="9de97-114">Boolean</span></span>|<span data-ttu-id="9de97-115">Se é para usar ou não o contexto de execução do dispositivo em aplicativo móvel da Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="9de97-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9de97-116">Relações</span><span class="sxs-lookup"><span data-stu-id="9de97-116">Relationships</span></span>
<span data-ttu-id="9de97-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9de97-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9de97-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9de97-118">JSON Representation</span></span>
<span data-ttu-id="9de97-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9de97-119">Here is a JSON representation of the resource.</span></span>
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





