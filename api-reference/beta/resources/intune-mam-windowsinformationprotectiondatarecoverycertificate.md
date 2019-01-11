---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f7b27bf766e17000f20679e86c006675f81e92bc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826840"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="400e2-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="400e2-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="400e2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="400e2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="400e2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="400e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="400e2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="400e2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="400e2-107">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="400e2-107">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="400e2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="400e2-108">Properties</span></span>
|<span data-ttu-id="400e2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="400e2-109">Property</span></span>|<span data-ttu-id="400e2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="400e2-110">Type</span></span>|<span data-ttu-id="400e2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="400e2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="400e2-112">SubjectName</span><span class="sxs-lookup"><span data-stu-id="400e2-112">subjectName</span></span>|<span data-ttu-id="400e2-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="400e2-113">String</span></span>|<span data-ttu-id="400e2-114">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="400e2-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="400e2-115">descrição</span><span class="sxs-lookup"><span data-stu-id="400e2-115">description</span></span>|<span data-ttu-id="400e2-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="400e2-116">String</span></span>|<span data-ttu-id="400e2-117">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="400e2-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="400e2-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="400e2-118">expirationDateTime</span></span>|<span data-ttu-id="400e2-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="400e2-119">DateTimeOffset</span></span>|<span data-ttu-id="400e2-120">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="400e2-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="400e2-121">certificado</span><span class="sxs-lookup"><span data-stu-id="400e2-121">certificate</span></span>|<span data-ttu-id="400e2-122">Binário</span><span class="sxs-lookup"><span data-stu-id="400e2-122">Binary</span></span>|<span data-ttu-id="400e2-123">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="400e2-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="400e2-124">Relações</span><span class="sxs-lookup"><span data-stu-id="400e2-124">Relationships</span></span>
<span data-ttu-id="400e2-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="400e2-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="400e2-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="400e2-126">JSON Representation</span></span>
<span data-ttu-id="400e2-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="400e2-127">Here is a JSON representation of the resource.</span></span>
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





