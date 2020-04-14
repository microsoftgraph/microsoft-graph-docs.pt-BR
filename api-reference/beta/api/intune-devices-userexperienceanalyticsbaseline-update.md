---
title: Atualizar userExperienceAnalyticsBaseline
description: Atualiza as propriedades de um objeto userExperienceAnalyticsBaseline.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f2de10d98ff3dccd875a53a6cb11e33690c442a5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43322744"
---
# <a name="update-userexperienceanalyticsbaseline"></a><span data-ttu-id="cecff-103">Atualizar userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="cecff-103">Update userExperienceAnalyticsBaseline</span></span>

<span data-ttu-id="cecff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cecff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cecff-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cecff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cecff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cecff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cecff-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) .</span><span class="sxs-lookup"><span data-stu-id="cecff-107">Update the properties of a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cecff-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cecff-108">Prerequisites</span></span>
<span data-ttu-id="cecff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cecff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cecff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cecff-111">Permission type</span></span>|<span data-ttu-id="cecff-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cecff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cecff-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cecff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cecff-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cecff-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cecff-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cecff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cecff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cecff-116">Not supported.</span></span>|
|<span data-ttu-id="cecff-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cecff-117">Application</span></span>|<span data-ttu-id="cecff-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cecff-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cecff-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cecff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
```

## <a name="request-headers"></a><span data-ttu-id="cecff-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cecff-120">Request headers</span></span>
|<span data-ttu-id="cecff-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cecff-121">Header</span></span>|<span data-ttu-id="cecff-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cecff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cecff-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cecff-123">Authorization</span></span>|<span data-ttu-id="cecff-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cecff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cecff-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cecff-125">Accept</span></span>|<span data-ttu-id="cecff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cecff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cecff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cecff-127">Request body</span></span>
<span data-ttu-id="cecff-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) .</span><span class="sxs-lookup"><span data-stu-id="cecff-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

<span data-ttu-id="cecff-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md).</span><span class="sxs-lookup"><span data-stu-id="cecff-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md).</span></span>

|<span data-ttu-id="cecff-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cecff-130">Property</span></span>|<span data-ttu-id="cecff-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cecff-131">Type</span></span>|<span data-ttu-id="cecff-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cecff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cecff-133">id</span><span class="sxs-lookup"><span data-stu-id="cecff-133">id</span></span>|<span data-ttu-id="cecff-134">String</span><span class="sxs-lookup"><span data-stu-id="cecff-134">String</span></span>|<span data-ttu-id="cecff-135">O identificador exclusivo da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="cecff-135">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="cecff-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cecff-136">displayName</span></span>|<span data-ttu-id="cecff-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cecff-137">String</span></span>|<span data-ttu-id="cecff-138">O nome da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="cecff-138">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="cecff-139">overallScore</span><span class="sxs-lookup"><span data-stu-id="cecff-139">overallScore</span></span>|<span data-ttu-id="cecff-140">Int32</span><span class="sxs-lookup"><span data-stu-id="cecff-140">Int32</span></span>|<span data-ttu-id="cecff-141">A pontuação geral da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="cecff-141">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="cecff-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="cecff-142">isBuiltIn</span></span>|<span data-ttu-id="cecff-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="cecff-143">Boolean</span></span>|<span data-ttu-id="cecff-144">Significa se a linha de base atual é a linha de base mediana comercial ou uma linha de base personalizada.</span><span class="sxs-lookup"><span data-stu-id="cecff-144">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="cecff-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cecff-145">createdDateTime</span></span>|<span data-ttu-id="cecff-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cecff-146">DateTimeOffset</span></span>|<span data-ttu-id="cecff-147">A data em que a linha de base personalizada foi criada.</span><span class="sxs-lookup"><span data-stu-id="cecff-147">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="cecff-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="cecff-148">Response</span></span>
<span data-ttu-id="cecff-149">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cecff-149">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cecff-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cecff-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="cecff-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cecff-151">Request</span></span>
<span data-ttu-id="cecff-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cecff-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cecff-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="cecff-153">Response</span></span>
<span data-ttu-id="cecff-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cecff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



