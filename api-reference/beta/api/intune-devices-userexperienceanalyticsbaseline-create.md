---
title: Criar userExperienceAnalyticsBaseline
description: Criar um novo objeto userExperienceAnalyticsBaseline.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3951869a6ec5f425fe9a37b62bb2d8c9261bf31b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691663"
---
# <a name="create-userexperienceanalyticsbaseline"></a><span data-ttu-id="19f00-103">Criar userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="19f00-103">Create userExperienceAnalyticsBaseline</span></span>

<span data-ttu-id="19f00-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19f00-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19f00-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="19f00-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19f00-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="19f00-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19f00-107">Criar um novo objeto [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) .</span><span class="sxs-lookup"><span data-stu-id="19f00-107">Create a new [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19f00-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="19f00-108">Prerequisites</span></span>
<span data-ttu-id="19f00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19f00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19f00-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19f00-111">Permission type</span></span>|<span data-ttu-id="19f00-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="19f00-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19f00-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19f00-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19f00-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19f00-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="19f00-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19f00-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19f00-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19f00-116">Not supported.</span></span>|
|<span data-ttu-id="19f00-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19f00-117">Application</span></span>|<span data-ttu-id="19f00-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19f00-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19f00-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19f00-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBaselines
```

## <a name="request-headers"></a><span data-ttu-id="19f00-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19f00-120">Request headers</span></span>
|<span data-ttu-id="19f00-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19f00-121">Header</span></span>|<span data-ttu-id="19f00-122">Valor</span><span class="sxs-lookup"><span data-stu-id="19f00-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19f00-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="19f00-123">Authorization</span></span>|<span data-ttu-id="19f00-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19f00-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19f00-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="19f00-125">Accept</span></span>|<span data-ttu-id="19f00-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19f00-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19f00-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19f00-127">Request body</span></span>
<span data-ttu-id="19f00-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsBaseline.</span><span class="sxs-lookup"><span data-stu-id="19f00-128">In the request body, supply a JSON representation for the userExperienceAnalyticsBaseline object.</span></span>

<span data-ttu-id="19f00-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsBaseline.</span><span class="sxs-lookup"><span data-stu-id="19f00-129">The following table shows the properties that are required when you create the userExperienceAnalyticsBaseline.</span></span>

|<span data-ttu-id="19f00-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19f00-130">Property</span></span>|<span data-ttu-id="19f00-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="19f00-131">Type</span></span>|<span data-ttu-id="19f00-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="19f00-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19f00-133">id</span><span class="sxs-lookup"><span data-stu-id="19f00-133">id</span></span>|<span data-ttu-id="19f00-134">String</span><span class="sxs-lookup"><span data-stu-id="19f00-134">String</span></span>|<span data-ttu-id="19f00-135">O identificador exclusivo da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="19f00-135">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="19f00-136">displayName</span><span class="sxs-lookup"><span data-stu-id="19f00-136">displayName</span></span>|<span data-ttu-id="19f00-137">String</span><span class="sxs-lookup"><span data-stu-id="19f00-137">String</span></span>|<span data-ttu-id="19f00-138">O nome da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="19f00-138">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="19f00-139">overallScore</span><span class="sxs-lookup"><span data-stu-id="19f00-139">overallScore</span></span>|<span data-ttu-id="19f00-140">Int32</span><span class="sxs-lookup"><span data-stu-id="19f00-140">Int32</span></span>|<span data-ttu-id="19f00-141">A pontuação geral da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="19f00-141">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="19f00-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="19f00-142">isBuiltIn</span></span>|<span data-ttu-id="19f00-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="19f00-143">Boolean</span></span>|<span data-ttu-id="19f00-144">Significa se a linha de base atual é a linha de base mediana comercial ou uma linha de base personalizada.</span><span class="sxs-lookup"><span data-stu-id="19f00-144">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="19f00-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19f00-145">createdDateTime</span></span>|<span data-ttu-id="19f00-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19f00-146">DateTimeOffset</span></span>|<span data-ttu-id="19f00-147">A data em que a linha de base personalizada foi criada.</span><span class="sxs-lookup"><span data-stu-id="19f00-147">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="19f00-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="19f00-148">Response</span></span>
<span data-ttu-id="19f00-149">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19f00-149">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19f00-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19f00-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="19f00-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19f00-151">Request</span></span>
<span data-ttu-id="19f00-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19f00-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "displayName": "Display Name value",
  "overallScore": 12,
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="19f00-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="19f00-153">Response</span></span>
<span data-ttu-id="19f00-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19f00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





