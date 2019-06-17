---
title: tipo de recurso managementCertificateWithThumbprint
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f497780f9ccd21ea608a8c7e56e6926d79263e24
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963475"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="0fac7-103">tipo de recurso managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="0fac7-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="0fac7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0fac7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fac7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0fac7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fac7-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0fac7-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0fac7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0fac7-107">Properties</span></span>
|<span data-ttu-id="0fac7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0fac7-108">Property</span></span>|<span data-ttu-id="0fac7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0fac7-109">Type</span></span>|<span data-ttu-id="0fac7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fac7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fac7-111">identificação</span><span class="sxs-lookup"><span data-stu-id="0fac7-111">thumbprint</span></span>|<span data-ttu-id="0fac7-112">String</span><span class="sxs-lookup"><span data-stu-id="0fac7-112">String</span></span>|<span data-ttu-id="0fac7-113">A impressão digital do certificado de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="0fac7-113">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="0fac7-114">certificado</span><span class="sxs-lookup"><span data-stu-id="0fac7-114">certificate</span></span>|<span data-ttu-id="0fac7-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0fac7-115">String</span></span>|<span data-ttu-id="0fac7-116">O certificado de gerenciamento codificado base 64</span><span class="sxs-lookup"><span data-stu-id="0fac7-116">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fac7-117">Relações</span><span class="sxs-lookup"><span data-stu-id="0fac7-117">Relationships</span></span>
<span data-ttu-id="0fac7-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0fac7-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fac7-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0fac7-119">JSON Representation</span></span>
<span data-ttu-id="0fac7-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0fac7-120">Here is a JSON representation of the resource.</span></span>
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





