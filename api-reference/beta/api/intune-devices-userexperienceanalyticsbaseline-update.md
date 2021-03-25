---
title: Atualizar userExperienceAnalyticsBaseline
description: Atualize as propriedades de um objeto userExperienceAnalyticsBaseline.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4594b56e33ff8cf7d8583c1233d5e0083bf6bcd1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154284"
---
# <a name="update-userexperienceanalyticsbaseline"></a><span data-ttu-id="7d334-103">Atualizar userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="7d334-103">Update userExperienceAnalyticsBaseline</span></span>

<span data-ttu-id="7d334-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d334-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d334-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7d334-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d334-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d334-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d334-107">Atualize as propriedades de [um objeto userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)</span><span class="sxs-lookup"><span data-stu-id="7d334-107">Update the properties of a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d334-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d334-108">Prerequisites</span></span>
<span data-ttu-id="7d334-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d334-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d334-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d334-111">Permission type</span></span>|<span data-ttu-id="7d334-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d334-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d334-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d334-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d334-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d334-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7d334-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d334-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d334-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d334-116">Not supported.</span></span>|
|<span data-ttu-id="7d334-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d334-117">Application</span></span>|<span data-ttu-id="7d334-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d334-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d334-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d334-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
```

## <a name="request-headers"></a><span data-ttu-id="7d334-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d334-120">Request headers</span></span>
|<span data-ttu-id="7d334-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d334-121">Header</span></span>|<span data-ttu-id="7d334-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7d334-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d334-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d334-123">Authorization</span></span>|<span data-ttu-id="7d334-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d334-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d334-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d334-125">Accept</span></span>|<span data-ttu-id="7d334-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d334-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d334-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d334-127">Request body</span></span>
<span data-ttu-id="7d334-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsBaseline.](../resources/intune-devices-userexperienceanalyticsbaseline.md)</span><span class="sxs-lookup"><span data-stu-id="7d334-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

<span data-ttu-id="7d334-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md).</span><span class="sxs-lookup"><span data-stu-id="7d334-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md).</span></span>

|<span data-ttu-id="7d334-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d334-130">Property</span></span>|<span data-ttu-id="7d334-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d334-131">Type</span></span>|<span data-ttu-id="7d334-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d334-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d334-133">id</span><span class="sxs-lookup"><span data-stu-id="7d334-133">id</span></span>|<span data-ttu-id="7d334-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d334-134">String</span></span>|<span data-ttu-id="7d334-135">O identificador exclusivo da linha de base de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="7d334-135">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="7d334-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7d334-136">displayName</span></span>|<span data-ttu-id="7d334-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d334-137">String</span></span>|<span data-ttu-id="7d334-138">O nome da linha de base de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="7d334-138">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="7d334-139">overallScore</span><span class="sxs-lookup"><span data-stu-id="7d334-139">overallScore</span></span>|<span data-ttu-id="7d334-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7d334-140">Int32</span></span>|<span data-ttu-id="7d334-141">A pontuação geral da linha de base de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="7d334-141">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="7d334-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="7d334-142">isBuiltIn</span></span>|<span data-ttu-id="7d334-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d334-143">Boolean</span></span>|<span data-ttu-id="7d334-144">Significa se a linha de base atual é a linha de base mediana comercial ou uma linha de base personalizada.</span><span class="sxs-lookup"><span data-stu-id="7d334-144">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="7d334-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d334-145">createdDateTime</span></span>|<span data-ttu-id="7d334-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d334-146">DateTimeOffset</span></span>|<span data-ttu-id="7d334-147">A data em que a linha de base personalizada foi criada.</span><span class="sxs-lookup"><span data-stu-id="7d334-147">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="7d334-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d334-148">Response</span></span>
<span data-ttu-id="7d334-149">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d334-149">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d334-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d334-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d334-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d334-151">Request</span></span>
<span data-ttu-id="7d334-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d334-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d334-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d334-153">Response</span></span>
<span data-ttu-id="7d334-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d334-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




