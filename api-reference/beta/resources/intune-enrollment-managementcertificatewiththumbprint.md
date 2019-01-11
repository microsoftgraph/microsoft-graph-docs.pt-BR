---
title: tipo de recurso de managementCertificateWithThumbprint
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d8f18e7fc117f00f99346267f544abc7d12db17e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827213"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="5de61-103">tipo de recurso de managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="5de61-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="5de61-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5de61-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5de61-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5de61-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5de61-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5de61-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5de61-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5de61-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="5de61-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5de61-108">Properties</span></span>
|<span data-ttu-id="5de61-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5de61-109">Property</span></span>|<span data-ttu-id="5de61-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5de61-110">Type</span></span>|<span data-ttu-id="5de61-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5de61-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5de61-112">impressão digital</span><span class="sxs-lookup"><span data-stu-id="5de61-112">thumbprint</span></span>|<span data-ttu-id="5de61-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5de61-113">String</span></span>|<span data-ttu-id="5de61-114">A impressão digital do certificado gerenciamento</span><span class="sxs-lookup"><span data-stu-id="5de61-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="5de61-115">certificado</span><span class="sxs-lookup"><span data-stu-id="5de61-115">certificate</span></span>|<span data-ttu-id="5de61-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5de61-116">String</span></span>|<span data-ttu-id="5de61-117">O certificado de gerenciamento codificada de Base 64</span><span class="sxs-lookup"><span data-stu-id="5de61-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="5de61-118">Relações</span><span class="sxs-lookup"><span data-stu-id="5de61-118">Relationships</span></span>
<span data-ttu-id="5de61-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5de61-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5de61-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5de61-120">JSON Representation</span></span>
<span data-ttu-id="5de61-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5de61-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCertificateWithThumbprint",
  "thumbprint": "String",
  "certificate": "String"
}
```





