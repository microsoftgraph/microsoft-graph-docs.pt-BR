---
title: Atualizar userExperienceAnalyticsBaseline
description: Atualiza as propriedades de um objeto userExperienceAnalyticsBaseline.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f8a91c0b0a70437d2a2ccee39d8afdd35d73aee
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944530"
---
# <a name="update-userexperienceanalyticsbaseline"></a><span data-ttu-id="a19be-103">Atualizar userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="a19be-103">Update userExperienceAnalyticsBaseline</span></span>

> <span data-ttu-id="a19be-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a19be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a19be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a19be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a19be-106">Atualiza as propriedades de um objeto [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) .</span><span class="sxs-lookup"><span data-stu-id="a19be-106">Update the properties of a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a19be-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a19be-107">Prerequisites</span></span>
<span data-ttu-id="a19be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a19be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a19be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a19be-110">Permission type</span></span>|<span data-ttu-id="a19be-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a19be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a19be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a19be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a19be-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a19be-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a19be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a19be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a19be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a19be-115">Not supported.</span></span>|
|<span data-ttu-id="a19be-116">Application</span><span class="sxs-lookup"><span data-stu-id="a19be-116">Application</span></span>|<span data-ttu-id="a19be-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a19be-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a19be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a19be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
```

## <a name="request-headers"></a><span data-ttu-id="a19be-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a19be-119">Request headers</span></span>
|<span data-ttu-id="a19be-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a19be-120">Header</span></span>|<span data-ttu-id="a19be-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a19be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a19be-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a19be-122">Authorization</span></span>|<span data-ttu-id="a19be-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a19be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a19be-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a19be-124">Accept</span></span>|<span data-ttu-id="a19be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a19be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a19be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a19be-126">Request body</span></span>
<span data-ttu-id="a19be-127">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) .</span><span class="sxs-lookup"><span data-stu-id="a19be-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

<span data-ttu-id="a19be-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md).</span><span class="sxs-lookup"><span data-stu-id="a19be-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md).</span></span>

|<span data-ttu-id="a19be-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a19be-129">Property</span></span>|<span data-ttu-id="a19be-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a19be-130">Type</span></span>|<span data-ttu-id="a19be-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a19be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a19be-132">id</span><span class="sxs-lookup"><span data-stu-id="a19be-132">id</span></span>|<span data-ttu-id="a19be-133">String</span><span class="sxs-lookup"><span data-stu-id="a19be-133">String</span></span>|<span data-ttu-id="a19be-134">O identificador exclusivo da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a19be-134">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="a19be-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a19be-135">displayName</span></span>|<span data-ttu-id="a19be-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a19be-136">String</span></span>|<span data-ttu-id="a19be-137">O nome da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a19be-137">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="a19be-138">overallScore</span><span class="sxs-lookup"><span data-stu-id="a19be-138">overallScore</span></span>|<span data-ttu-id="a19be-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a19be-139">Int32</span></span>|<span data-ttu-id="a19be-140">A pontuação geral da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a19be-140">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="a19be-141">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="a19be-141">isBuiltIn</span></span>|<span data-ttu-id="a19be-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="a19be-142">Boolean</span></span>|<span data-ttu-id="a19be-143">Significa se a linha de base atual é a linha de base mediana comercial ou uma linha de base personalizada.</span><span class="sxs-lookup"><span data-stu-id="a19be-143">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="a19be-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a19be-144">createdDateTime</span></span>|<span data-ttu-id="a19be-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a19be-145">DateTimeOffset</span></span>|<span data-ttu-id="a19be-146">A data em que a linha de base personalizada foi criada.</span><span class="sxs-lookup"><span data-stu-id="a19be-146">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="a19be-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="a19be-147">Response</span></span>
<span data-ttu-id="a19be-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a19be-148">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a19be-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a19be-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="a19be-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a19be-150">Request</span></span>
<span data-ttu-id="a19be-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a19be-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "displayName": "Display Name value",
  "overallScore": 12,
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="a19be-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="a19be-152">Response</span></span>
<span data-ttu-id="a19be-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a19be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 266

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "1cce2cab-2cab-1cce-ab2c-ce1cab2cce1c",
  "displayName": "Display Name value",
  "overallScore": 12,
  "isBuiltIn": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00"
}
```





