---
title: Criar userExperienceAnalyticsBaseline
description: Criar um novo objeto userExperienceAnalyticsBaseline.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8c6b1472fcee0f38c561be44685b2583f0d6fc1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072323"
---
# <a name="create-userexperienceanalyticsbaseline"></a><span data-ttu-id="56409-103">Criar userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="56409-103">Create userExperienceAnalyticsBaseline</span></span>

<span data-ttu-id="56409-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56409-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56409-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="56409-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56409-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="56409-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56409-107">Criar um novo objeto [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) .</span><span class="sxs-lookup"><span data-stu-id="56409-107">Create a new [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56409-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="56409-108">Prerequisites</span></span>
<span data-ttu-id="56409-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56409-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56409-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56409-111">Permission type</span></span>|<span data-ttu-id="56409-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="56409-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56409-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56409-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56409-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56409-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="56409-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56409-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56409-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56409-116">Not supported.</span></span>|
|<span data-ttu-id="56409-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56409-117">Application</span></span>|<span data-ttu-id="56409-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56409-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56409-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56409-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBaselines
```

## <a name="request-headers"></a><span data-ttu-id="56409-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56409-120">Request headers</span></span>
|<span data-ttu-id="56409-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56409-121">Header</span></span>|<span data-ttu-id="56409-122">Valor</span><span class="sxs-lookup"><span data-stu-id="56409-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56409-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="56409-123">Authorization</span></span>|<span data-ttu-id="56409-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56409-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56409-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="56409-125">Accept</span></span>|<span data-ttu-id="56409-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56409-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56409-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56409-127">Request body</span></span>
<span data-ttu-id="56409-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsBaseline.</span><span class="sxs-lookup"><span data-stu-id="56409-128">In the request body, supply a JSON representation for the userExperienceAnalyticsBaseline object.</span></span>

<span data-ttu-id="56409-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsBaseline.</span><span class="sxs-lookup"><span data-stu-id="56409-129">The following table shows the properties that are required when you create the userExperienceAnalyticsBaseline.</span></span>

|<span data-ttu-id="56409-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56409-130">Property</span></span>|<span data-ttu-id="56409-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="56409-131">Type</span></span>|<span data-ttu-id="56409-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="56409-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56409-133">id</span><span class="sxs-lookup"><span data-stu-id="56409-133">id</span></span>|<span data-ttu-id="56409-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56409-134">String</span></span>|<span data-ttu-id="56409-135">O identificador exclusivo da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="56409-135">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="56409-136">displayName</span><span class="sxs-lookup"><span data-stu-id="56409-136">displayName</span></span>|<span data-ttu-id="56409-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56409-137">String</span></span>|<span data-ttu-id="56409-138">O nome da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="56409-138">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="56409-139">overallScore</span><span class="sxs-lookup"><span data-stu-id="56409-139">overallScore</span></span>|<span data-ttu-id="56409-140">Int32</span><span class="sxs-lookup"><span data-stu-id="56409-140">Int32</span></span>|<span data-ttu-id="56409-141">A pontuação geral da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="56409-141">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="56409-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="56409-142">isBuiltIn</span></span>|<span data-ttu-id="56409-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="56409-143">Boolean</span></span>|<span data-ttu-id="56409-144">Significa se a linha de base atual é a linha de base mediana comercial ou uma linha de base personalizada.</span><span class="sxs-lookup"><span data-stu-id="56409-144">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="56409-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56409-145">createdDateTime</span></span>|<span data-ttu-id="56409-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56409-146">DateTimeOffset</span></span>|<span data-ttu-id="56409-147">A data em que a linha de base personalizada foi criada.</span><span class="sxs-lookup"><span data-stu-id="56409-147">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="56409-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="56409-148">Response</span></span>
<span data-ttu-id="56409-149">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56409-149">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56409-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56409-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="56409-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56409-151">Request</span></span>
<span data-ttu-id="56409-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56409-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="56409-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="56409-153">Response</span></span>
<span data-ttu-id="56409-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56409-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






