---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 72edbdc16b2d84a2df6a4582bba12bab2feaa04c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821060"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="bee08-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="bee08-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="bee08-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bee08-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bee08-105">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="bee08-105">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="bee08-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bee08-106">Properties</span></span>
|<span data-ttu-id="bee08-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bee08-107">Property</span></span>|<span data-ttu-id="bee08-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bee08-108">Type</span></span>|<span data-ttu-id="bee08-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bee08-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bee08-110">SubjectName</span><span class="sxs-lookup"><span data-stu-id="bee08-110">subjectName</span></span>|<span data-ttu-id="bee08-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bee08-111">String</span></span>|<span data-ttu-id="bee08-112">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="bee08-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="bee08-113">descrição</span><span class="sxs-lookup"><span data-stu-id="bee08-113">description</span></span>|<span data-ttu-id="bee08-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bee08-114">String</span></span>|<span data-ttu-id="bee08-115">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="bee08-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="bee08-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bee08-116">expirationDateTime</span></span>|<span data-ttu-id="bee08-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bee08-117">DateTimeOffset</span></span>|<span data-ttu-id="bee08-118">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="bee08-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="bee08-119">certificado</span><span class="sxs-lookup"><span data-stu-id="bee08-119">certificate</span></span>|<span data-ttu-id="bee08-120">Binário</span><span class="sxs-lookup"><span data-stu-id="bee08-120">Binary</span></span>|<span data-ttu-id="bee08-121">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="bee08-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="bee08-122">Relações</span><span class="sxs-lookup"><span data-stu-id="bee08-122">Relationships</span></span>
<span data-ttu-id="bee08-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bee08-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bee08-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bee08-124">JSON Representation</span></span>
<span data-ttu-id="bee08-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bee08-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```



