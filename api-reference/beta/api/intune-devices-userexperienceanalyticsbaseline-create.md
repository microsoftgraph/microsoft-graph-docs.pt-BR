---
title: Criar userExperienceAnalyticsBaseline
description: Crie um novo objeto userExperienceAnalyticsBaseline.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4887e2d15e1a8d1b89dab3b72aa53344f499d523
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157958"
---
# <a name="create-userexperienceanalyticsbaseline"></a><span data-ttu-id="b862a-103">Criar userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="b862a-103">Create userExperienceAnalyticsBaseline</span></span>

<span data-ttu-id="b862a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b862a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b862a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b862a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b862a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b862a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b862a-107">Crie um novo [objeto userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)</span><span class="sxs-lookup"><span data-stu-id="b862a-107">Create a new [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b862a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b862a-108">Prerequisites</span></span>
<span data-ttu-id="b862a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b862a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b862a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b862a-111">Permission type</span></span>|<span data-ttu-id="b862a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b862a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b862a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b862a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b862a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b862a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b862a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b862a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b862a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b862a-116">Not supported.</span></span>|
|<span data-ttu-id="b862a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b862a-117">Application</span></span>|<span data-ttu-id="b862a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b862a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b862a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b862a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBaselines
```

## <a name="request-headers"></a><span data-ttu-id="b862a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b862a-120">Request headers</span></span>
|<span data-ttu-id="b862a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b862a-121">Header</span></span>|<span data-ttu-id="b862a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b862a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b862a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b862a-123">Authorization</span></span>|<span data-ttu-id="b862a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b862a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b862a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b862a-125">Accept</span></span>|<span data-ttu-id="b862a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b862a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b862a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b862a-127">Request body</span></span>
<span data-ttu-id="b862a-128">No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsBaseline.</span><span class="sxs-lookup"><span data-stu-id="b862a-128">In the request body, supply a JSON representation for the userExperienceAnalyticsBaseline object.</span></span>

<span data-ttu-id="b862a-129">A tabela a seguir mostra as propriedades necessárias ao criar o userExperienceAnalyticsBaseline.</span><span class="sxs-lookup"><span data-stu-id="b862a-129">The following table shows the properties that are required when you create the userExperienceAnalyticsBaseline.</span></span>

|<span data-ttu-id="b862a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b862a-130">Property</span></span>|<span data-ttu-id="b862a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b862a-131">Type</span></span>|<span data-ttu-id="b862a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b862a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b862a-133">id</span><span class="sxs-lookup"><span data-stu-id="b862a-133">id</span></span>|<span data-ttu-id="b862a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b862a-134">String</span></span>|<span data-ttu-id="b862a-135">O identificador exclusivo da linha de base de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="b862a-135">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="b862a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b862a-136">displayName</span></span>|<span data-ttu-id="b862a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b862a-137">String</span></span>|<span data-ttu-id="b862a-138">O nome da linha de base de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="b862a-138">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="b862a-139">overallScore</span><span class="sxs-lookup"><span data-stu-id="b862a-139">overallScore</span></span>|<span data-ttu-id="b862a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b862a-140">Int32</span></span>|<span data-ttu-id="b862a-141">A pontuação geral da linha de base de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="b862a-141">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="b862a-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="b862a-142">isBuiltIn</span></span>|<span data-ttu-id="b862a-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="b862a-143">Boolean</span></span>|<span data-ttu-id="b862a-144">Significa se a linha de base atual é a linha de base mediana comercial ou uma linha de base personalizada.</span><span class="sxs-lookup"><span data-stu-id="b862a-144">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="b862a-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b862a-145">createdDateTime</span></span>|<span data-ttu-id="b862a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b862a-146">DateTimeOffset</span></span>|<span data-ttu-id="b862a-147">A data em que a linha de base personalizada foi criada.</span><span class="sxs-lookup"><span data-stu-id="b862a-147">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="b862a-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b862a-148">Response</span></span>
<span data-ttu-id="b862a-149">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b862a-149">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b862a-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b862a-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="b862a-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b862a-151">Request</span></span>
<span data-ttu-id="b862a-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b862a-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b862a-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b862a-153">Response</span></span>
<span data-ttu-id="b862a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b862a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




