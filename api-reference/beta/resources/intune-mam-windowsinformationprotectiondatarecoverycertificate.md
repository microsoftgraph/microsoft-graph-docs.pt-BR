---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5e686ab1a6c1e586c8bd32c56d3480102503b4be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976251"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="97f9e-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="97f9e-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="97f9e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="97f9e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97f9e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="97f9e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97f9e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="97f9e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97f9e-107">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="97f9e-107">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="97f9e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97f9e-108">Properties</span></span>
|<span data-ttu-id="97f9e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97f9e-109">Property</span></span>|<span data-ttu-id="97f9e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="97f9e-110">Type</span></span>|<span data-ttu-id="97f9e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="97f9e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97f9e-112">SubjectName</span><span class="sxs-lookup"><span data-stu-id="97f9e-112">subjectName</span></span>|<span data-ttu-id="97f9e-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97f9e-113">String</span></span>|<span data-ttu-id="97f9e-114">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="97f9e-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="97f9e-115">descrição</span><span class="sxs-lookup"><span data-stu-id="97f9e-115">description</span></span>|<span data-ttu-id="97f9e-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97f9e-116">String</span></span>|<span data-ttu-id="97f9e-117">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="97f9e-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="97f9e-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="97f9e-118">expirationDateTime</span></span>|<span data-ttu-id="97f9e-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97f9e-119">DateTimeOffset</span></span>|<span data-ttu-id="97f9e-120">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="97f9e-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="97f9e-121">certificado</span><span class="sxs-lookup"><span data-stu-id="97f9e-121">certificate</span></span>|<span data-ttu-id="97f9e-122">Binário</span><span class="sxs-lookup"><span data-stu-id="97f9e-122">Binary</span></span>|<span data-ttu-id="97f9e-123">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="97f9e-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="97f9e-124">Relações</span><span class="sxs-lookup"><span data-stu-id="97f9e-124">Relationships</span></span>
<span data-ttu-id="97f9e-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97f9e-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="97f9e-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97f9e-126">JSON Representation</span></span>
<span data-ttu-id="97f9e-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97f9e-127">Here is a JSON representation of the resource.</span></span>
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





