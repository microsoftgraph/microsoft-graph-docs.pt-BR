---
title: tipo de recurso de windowsKioskActiveDirectoryGroup
description: A classe usada para identificar um grupo de diretório do Windows Azure para a configuração de quiosque
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dc9db9aa120411c423492efa162973e33cc4c303
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850523"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="6c6fc-103">tipo de recurso de windowsKioskActiveDirectoryGroup</span><span class="sxs-lookup"><span data-stu-id="6c6fc-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="6c6fc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6c6fc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c6fc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6c6fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c6fc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6c6fc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c6fc-107">A classe usada para identificar um grupo de diretório do Windows Azure para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="6c6fc-107">The class used to identify an Azure Directory group for the kiosk configuration</span></span>

<span data-ttu-id="6c6fc-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="6c6fc-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6c6fc-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c6fc-109">Properties</span></span>
|<span data-ttu-id="6c6fc-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c6fc-110">Property</span></span>|<span data-ttu-id="6c6fc-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c6fc-111">Type</span></span>|<span data-ttu-id="6c6fc-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c6fc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c6fc-113">groupName</span><span class="sxs-lookup"><span data-stu-id="6c6fc-113">groupName</span></span>|<span data-ttu-id="6c6fc-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c6fc-114">String</span></span>|<span data-ttu-id="6c6fc-115">O nome do grupo AD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="6c6fc-115">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c6fc-116">Relações</span><span class="sxs-lookup"><span data-stu-id="6c6fc-116">Relationships</span></span>
<span data-ttu-id="6c6fc-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c6fc-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6c6fc-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c6fc-118">JSON Representation</span></span>
<span data-ttu-id="6c6fc-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c6fc-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskActiveDirectoryGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskActiveDirectoryGroup",
  "groupName": "String"
}
```





