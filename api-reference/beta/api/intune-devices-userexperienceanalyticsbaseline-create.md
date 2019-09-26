---
title: Criar userExperienceAnalyticsBaseline
description: Criar um novo objeto userExperienceAnalyticsBaseline.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6d9cadb07ac467c8390252820fd5d785a94280d1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37180206"
---
# <a name="create-userexperienceanalyticsbaseline"></a><span data-ttu-id="89315-103">Criar userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="89315-103">Create userExperienceAnalyticsBaseline</span></span>

> <span data-ttu-id="89315-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="89315-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89315-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89315-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89315-106">Criar um novo objeto [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) .</span><span class="sxs-lookup"><span data-stu-id="89315-106">Create a new [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89315-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89315-107">Prerequisites</span></span>
<span data-ttu-id="89315-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89315-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89315-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89315-110">Permission type</span></span>|<span data-ttu-id="89315-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="89315-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89315-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89315-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89315-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89315-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="89315-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89315-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89315-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89315-115">Not supported.</span></span>|
|<span data-ttu-id="89315-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89315-116">Application</span></span>|<span data-ttu-id="89315-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89315-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89315-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89315-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBaselines
```

## <a name="request-headers"></a><span data-ttu-id="89315-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89315-119">Request headers</span></span>
|<span data-ttu-id="89315-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89315-120">Header</span></span>|<span data-ttu-id="89315-121">Valor</span><span class="sxs-lookup"><span data-stu-id="89315-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89315-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="89315-122">Authorization</span></span>|<span data-ttu-id="89315-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89315-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89315-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="89315-124">Accept</span></span>|<span data-ttu-id="89315-125">application/json</span><span class="sxs-lookup"><span data-stu-id="89315-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89315-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89315-126">Request body</span></span>
<span data-ttu-id="89315-127">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsBaseline.</span><span class="sxs-lookup"><span data-stu-id="89315-127">In the request body, supply a JSON representation for the userExperienceAnalyticsBaseline object.</span></span>

<span data-ttu-id="89315-128">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsBaseline.</span><span class="sxs-lookup"><span data-stu-id="89315-128">The following table shows the properties that are required when you create the userExperienceAnalyticsBaseline.</span></span>

|<span data-ttu-id="89315-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89315-129">Property</span></span>|<span data-ttu-id="89315-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="89315-130">Type</span></span>|<span data-ttu-id="89315-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="89315-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89315-132">id</span><span class="sxs-lookup"><span data-stu-id="89315-132">id</span></span>|<span data-ttu-id="89315-133">String</span><span class="sxs-lookup"><span data-stu-id="89315-133">String</span></span>|<span data-ttu-id="89315-134">O identificador exclusivo da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="89315-134">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="89315-135">displayName</span><span class="sxs-lookup"><span data-stu-id="89315-135">displayName</span></span>|<span data-ttu-id="89315-136">String</span><span class="sxs-lookup"><span data-stu-id="89315-136">String</span></span>|<span data-ttu-id="89315-137">O nome da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="89315-137">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="89315-138">overallScore</span><span class="sxs-lookup"><span data-stu-id="89315-138">overallScore</span></span>|<span data-ttu-id="89315-139">Int32</span><span class="sxs-lookup"><span data-stu-id="89315-139">Int32</span></span>|<span data-ttu-id="89315-140">A pontuação geral da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="89315-140">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="89315-141">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="89315-141">isBuiltIn</span></span>|<span data-ttu-id="89315-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="89315-142">Boolean</span></span>|<span data-ttu-id="89315-143">Significa se a linha de base atual é a linha de base mediana comercial ou uma linha de base personalizada.</span><span class="sxs-lookup"><span data-stu-id="89315-143">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="89315-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89315-144">createdDateTime</span></span>|<span data-ttu-id="89315-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89315-145">DateTimeOffset</span></span>|<span data-ttu-id="89315-146">A data em que a linha de base personalizada foi criada.</span><span class="sxs-lookup"><span data-stu-id="89315-146">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="89315-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="89315-147">Response</span></span>
<span data-ttu-id="89315-148">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89315-148">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89315-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89315-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="89315-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89315-150">Request</span></span>
<span data-ttu-id="89315-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89315-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="89315-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="89315-152">Response</span></span>
<span data-ttu-id="89315-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89315-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




