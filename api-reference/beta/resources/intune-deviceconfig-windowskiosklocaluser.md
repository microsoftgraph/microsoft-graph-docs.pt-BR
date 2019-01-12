---
title: tipo de recurso de windowsKioskLocalUser
description: A classe usada para identificar uma conta local para a configuração de quiosque
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2dc1e54f7bc4e9fbbef3113abce90cab00825be8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934629"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="8a707-103">tipo de recurso de windowsKioskLocalUser</span><span class="sxs-lookup"><span data-stu-id="8a707-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="8a707-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8a707-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a707-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8a707-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a707-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8a707-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a707-107">A classe usada para identificar uma conta local para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="8a707-107">The class used to identify a local account for the kiosk configuration</span></span>

<span data-ttu-id="8a707-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="8a707-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8a707-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8a707-109">Properties</span></span>
|<span data-ttu-id="8a707-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a707-110">Property</span></span>|<span data-ttu-id="8a707-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a707-111">Type</span></span>|<span data-ttu-id="8a707-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a707-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a707-113">userName</span><span class="sxs-lookup"><span data-stu-id="8a707-113">userName</span></span>|<span data-ttu-id="8a707-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a707-114">String</span></span>|<span data-ttu-id="8a707-115">O usuário local que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="8a707-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a707-116">Relações</span><span class="sxs-lookup"><span data-stu-id="8a707-116">Relationships</span></span>
<span data-ttu-id="8a707-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8a707-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8a707-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8a707-118">JSON Representation</span></span>
<span data-ttu-id="8a707-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8a707-119">Here is a JSON representation of the resource.</span></span>
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





