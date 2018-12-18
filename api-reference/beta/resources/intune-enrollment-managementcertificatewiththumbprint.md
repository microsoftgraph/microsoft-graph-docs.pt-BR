---
title: tipo de recurso de managementCertificateWithThumbprint
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 03846890822cae02a2eb04fc058895992119c98a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348934"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="61564-103">tipo de recurso de managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="61564-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="61564-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="61564-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61564-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="61564-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61564-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="61564-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61564-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="61564-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="61564-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61564-108">Properties</span></span>
|<span data-ttu-id="61564-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61564-109">Property</span></span>|<span data-ttu-id="61564-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="61564-110">Type</span></span>|<span data-ttu-id="61564-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="61564-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61564-112">impressão digital</span><span class="sxs-lookup"><span data-stu-id="61564-112">thumbprint</span></span>|<span data-ttu-id="61564-113">String</span><span class="sxs-lookup"><span data-stu-id="61564-113">String</span></span>|<span data-ttu-id="61564-114">A impressão digital do certificado gerenciamento</span><span class="sxs-lookup"><span data-stu-id="61564-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="61564-115">certificado</span><span class="sxs-lookup"><span data-stu-id="61564-115">certificate</span></span>|<span data-ttu-id="61564-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61564-116">String</span></span>|<span data-ttu-id="61564-117">O certificado de gerenciamento codificada de Base 64</span><span class="sxs-lookup"><span data-stu-id="61564-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="61564-118">Relações</span><span class="sxs-lookup"><span data-stu-id="61564-118">Relationships</span></span>
<span data-ttu-id="61564-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61564-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="61564-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61564-120">JSON Representation</span></span>
<span data-ttu-id="61564-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61564-121">Here is a JSON representation of the resource.</span></span>
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





