---
title: tipo de recurso de windowsKioskLocalUser
description: A classe usada para identificar uma conta local para a configuração de quiosque
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b808cdb6cb8bb8540a553104d2c00108341a3e14
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392665"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="99af6-103">tipo de recurso de windowsKioskLocalUser</span><span class="sxs-lookup"><span data-stu-id="99af6-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="99af6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="99af6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="99af6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="99af6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99af6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="99af6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99af6-107">A classe usada para identificar uma conta local para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="99af6-107">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="99af6-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="99af6-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="99af6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99af6-109">Properties</span></span>
|<span data-ttu-id="99af6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99af6-110">Property</span></span>|<span data-ttu-id="99af6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="99af6-111">Type</span></span>|<span data-ttu-id="99af6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="99af6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99af6-113">userName</span><span class="sxs-lookup"><span data-stu-id="99af6-113">userName</span></span>|<span data-ttu-id="99af6-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99af6-114">String</span></span>|<span data-ttu-id="99af6-115">O usuário local que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="99af6-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="99af6-116">Relações</span><span class="sxs-lookup"><span data-stu-id="99af6-116">Relationships</span></span>
<span data-ttu-id="99af6-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99af6-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99af6-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99af6-118">JSON Representation</span></span>
<span data-ttu-id="99af6-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99af6-119">Here is a JSON representation of the resource.</span></span>
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




