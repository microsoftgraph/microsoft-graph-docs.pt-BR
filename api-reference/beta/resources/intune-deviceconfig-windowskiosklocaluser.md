---
title: tipo de recurso de windowsKioskLocalUser
description: A classe usada para identificar uma conta local para a configuração de quiosque
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7ab6a9dc0e3ea63ed5d9f60bb48b005aa98acab1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844552"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="27074-103">tipo de recurso de windowsKioskLocalUser</span><span class="sxs-lookup"><span data-stu-id="27074-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="27074-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="27074-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27074-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="27074-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27074-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="27074-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27074-107">A classe usada para identificar uma conta local para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="27074-107">The class used to identify a local account for the kiosk configuration</span></span>

<span data-ttu-id="27074-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="27074-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="27074-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27074-109">Properties</span></span>
|<span data-ttu-id="27074-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27074-110">Property</span></span>|<span data-ttu-id="27074-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="27074-111">Type</span></span>|<span data-ttu-id="27074-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="27074-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27074-113">userName</span><span class="sxs-lookup"><span data-stu-id="27074-113">userName</span></span>|<span data-ttu-id="27074-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27074-114">String</span></span>|<span data-ttu-id="27074-115">O usuário local que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="27074-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="27074-116">Relações</span><span class="sxs-lookup"><span data-stu-id="27074-116">Relationships</span></span>
<span data-ttu-id="27074-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="27074-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="27074-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27074-118">JSON Representation</span></span>
<span data-ttu-id="27074-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="27074-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```





