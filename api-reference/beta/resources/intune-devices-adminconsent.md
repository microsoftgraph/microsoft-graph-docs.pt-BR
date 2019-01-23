---
title: tipo de recurso de adminConsent
description: Informações de consentimento do administrador.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c76ac169bb15792afec908f62b9740e81a4d7e5b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415877"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="317c2-103">tipo de recurso de adminConsent</span><span class="sxs-lookup"><span data-stu-id="317c2-103">adminConsent resource type</span></span>

> <span data-ttu-id="317c2-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="317c2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="317c2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="317c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="317c2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="317c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="317c2-107">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="317c2-107">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="317c2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="317c2-108">Properties</span></span>
|<span data-ttu-id="317c2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="317c2-109">Property</span></span>|<span data-ttu-id="317c2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="317c2-110">Type</span></span>|<span data-ttu-id="317c2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="317c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="317c2-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="317c2-112">shareAPNSData</span></span>|[<span data-ttu-id="317c2-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="317c2-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="317c2-114">O estado de consentimento de admin de compartilhamento de usuário e dados de dispositivo para Apple.</span><span class="sxs-lookup"><span data-stu-id="317c2-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="317c2-115">Os valores possíveis são: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="317c2-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="317c2-116">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="317c2-116">Relationships</span></span>
<span data-ttu-id="317c2-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="317c2-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="317c2-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="317c2-118">JSON Representation</span></span>
<span data-ttu-id="317c2-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="317c2-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String"
}
```




