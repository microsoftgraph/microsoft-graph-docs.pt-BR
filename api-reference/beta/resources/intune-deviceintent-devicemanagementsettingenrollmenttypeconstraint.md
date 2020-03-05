---
title: tipo de recurso deviceManagementSettingEnrollmentTypeConstraint
description: Restrição que impõe os tipos de inscrição aplicados a uma configuração
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cfea5505dc05ac037ced5d9b714edb53ed6f768d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528791"
---
# <a name="devicemanagementsettingenrollmenttypeconstraint-resource-type"></a><span data-ttu-id="88c60-103">tipo de recurso deviceManagementSettingEnrollmentTypeConstraint</span><span class="sxs-lookup"><span data-stu-id="88c60-103">deviceManagementSettingEnrollmentTypeConstraint resource type</span></span>

<span data-ttu-id="88c60-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="88c60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88c60-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88c60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88c60-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88c60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88c60-107">Restrição que impõe os tipos de inscrição aplicados a uma configuração</span><span class="sxs-lookup"><span data-stu-id="88c60-107">Constraint that enforces the enrollment types applied to a setting</span></span>


<span data-ttu-id="88c60-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="88c60-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="88c60-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88c60-109">Properties</span></span>
|<span data-ttu-id="88c60-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88c60-110">Property</span></span>|<span data-ttu-id="88c60-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="88c60-111">Type</span></span>|<span data-ttu-id="88c60-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="88c60-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88c60-113">enrollmentTypes</span><span class="sxs-lookup"><span data-stu-id="88c60-113">enrollmentTypes</span></span>|<span data-ttu-id="88c60-114">String collection</span><span class="sxs-lookup"><span data-stu-id="88c60-114">String collection</span></span>|<span data-ttu-id="88c60-115">Lista de tipos de registro</span><span class="sxs-lookup"><span data-stu-id="88c60-115">List of enrollment types</span></span>|

## <a name="relationships"></a><span data-ttu-id="88c60-116">Relações</span><span class="sxs-lookup"><span data-stu-id="88c60-116">Relationships</span></span>
<span data-ttu-id="88c60-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="88c60-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88c60-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88c60-118">JSON Representation</span></span>
<span data-ttu-id="88c60-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88c60-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingEnrollmentTypeConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingEnrollmentTypeConstraint",
  "enrollmentTypes": [
    "String"
  ]
}
```



