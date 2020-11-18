---
title: Criar userExperienceAnalyticsBaseline
description: Criar um novo objeto userExperienceAnalyticsBaseline.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f78a3f9684068d9859c91ed75c91507a50f01bc9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202532"
---
# <a name="create-userexperienceanalyticsbaseline"></a><span data-ttu-id="b26b6-103">Criar userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="b26b6-103">Create userExperienceAnalyticsBaseline</span></span>

<span data-ttu-id="b26b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b26b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b26b6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b26b6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b26b6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b26b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b26b6-107">Criar um novo objeto [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) .</span><span class="sxs-lookup"><span data-stu-id="b26b6-107">Create a new [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b26b6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b26b6-108">Prerequisites</span></span>
<span data-ttu-id="b26b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b26b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b26b6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b26b6-111">Permission type</span></span>|<span data-ttu-id="b26b6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b26b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b26b6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b26b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b26b6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b26b6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b26b6-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b26b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b26b6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b26b6-116">Not supported.</span></span>|
|<span data-ttu-id="b26b6-117">Application</span><span class="sxs-lookup"><span data-stu-id="b26b6-117">Application</span></span>|<span data-ttu-id="b26b6-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b26b6-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b26b6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b26b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBaselines
```

## <a name="request-headers"></a><span data-ttu-id="b26b6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b26b6-120">Request headers</span></span>
|<span data-ttu-id="b26b6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b26b6-121">Header</span></span>|<span data-ttu-id="b26b6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b26b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b26b6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b26b6-123">Authorization</span></span>|<span data-ttu-id="b26b6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b26b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b26b6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b26b6-125">Accept</span></span>|<span data-ttu-id="b26b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b26b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b26b6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b26b6-127">Request body</span></span>
<span data-ttu-id="b26b6-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsBaseline.</span><span class="sxs-lookup"><span data-stu-id="b26b6-128">In the request body, supply a JSON representation for the userExperienceAnalyticsBaseline object.</span></span>

<span data-ttu-id="b26b6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsBaseline.</span><span class="sxs-lookup"><span data-stu-id="b26b6-129">The following table shows the properties that are required when you create the userExperienceAnalyticsBaseline.</span></span>

|<span data-ttu-id="b26b6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b26b6-130">Property</span></span>|<span data-ttu-id="b26b6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b26b6-131">Type</span></span>|<span data-ttu-id="b26b6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b26b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b26b6-133">id</span><span class="sxs-lookup"><span data-stu-id="b26b6-133">id</span></span>|<span data-ttu-id="b26b6-134">String</span><span class="sxs-lookup"><span data-stu-id="b26b6-134">String</span></span>|<span data-ttu-id="b26b6-135">O identificador exclusivo da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="b26b6-135">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="b26b6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b26b6-136">displayName</span></span>|<span data-ttu-id="b26b6-137">String</span><span class="sxs-lookup"><span data-stu-id="b26b6-137">String</span></span>|<span data-ttu-id="b26b6-138">O nome da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="b26b6-138">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="b26b6-139">overallScore</span><span class="sxs-lookup"><span data-stu-id="b26b6-139">overallScore</span></span>|<span data-ttu-id="b26b6-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b26b6-140">Int32</span></span>|<span data-ttu-id="b26b6-141">A pontuação geral da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="b26b6-141">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="b26b6-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="b26b6-142">isBuiltIn</span></span>|<span data-ttu-id="b26b6-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="b26b6-143">Boolean</span></span>|<span data-ttu-id="b26b6-144">Significa se a linha de base atual é a linha de base mediana comercial ou uma linha de base personalizada.</span><span class="sxs-lookup"><span data-stu-id="b26b6-144">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="b26b6-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b26b6-145">createdDateTime</span></span>|<span data-ttu-id="b26b6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b26b6-146">DateTimeOffset</span></span>|<span data-ttu-id="b26b6-147">A data em que a linha de base personalizada foi criada.</span><span class="sxs-lookup"><span data-stu-id="b26b6-147">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="b26b6-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b26b6-148">Response</span></span>
<span data-ttu-id="b26b6-149">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b26b6-149">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b26b6-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b26b6-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="b26b6-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b26b6-151">Request</span></span>
<span data-ttu-id="b26b6-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b26b6-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b26b6-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b26b6-153">Response</span></span>
<span data-ttu-id="b26b6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b26b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




