---
title: tipo de recurso de managedDeviceReportedApp
description: Dados de aplicativo para relatórios
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 104503083f5f599bc366de2ca8082fd9fdf3102e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422604"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="4870f-103">tipo de recurso de managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="4870f-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="4870f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="4870f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4870f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4870f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4870f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="4870f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4870f-107">Dados de aplicativo para relatórios</span><span class="sxs-lookup"><span data-stu-id="4870f-107">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="4870f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4870f-108">Properties</span></span>
|<span data-ttu-id="4870f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4870f-109">Property</span></span>|<span data-ttu-id="4870f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4870f-110">Type</span></span>|<span data-ttu-id="4870f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4870f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4870f-112">appId</span><span class="sxs-lookup"><span data-stu-id="4870f-112">appId</span></span>|<span data-ttu-id="4870f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4870f-113">String</span></span>|<span data-ttu-id="4870f-114">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4870f-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="4870f-115">Relações</span><span class="sxs-lookup"><span data-stu-id="4870f-115">Relationships</span></span>
<span data-ttu-id="4870f-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4870f-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4870f-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4870f-117">JSON Representation</span></span>
<span data-ttu-id="4870f-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4870f-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceReportedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceReportedApp",
  "appId": "String"
}
```




