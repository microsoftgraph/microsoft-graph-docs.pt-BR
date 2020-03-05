---
title: Criar userExperienceAnalyticsBaseline
description: Criar um novo objeto userExperienceAnalyticsBaseline.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14191e3b35ff1854eb8d7b14793991da1b31537c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468583"
---
# <a name="create-userexperienceanalyticsbaseline"></a><span data-ttu-id="3af59-103">Criar userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="3af59-103">Create userExperienceAnalyticsBaseline</span></span>

<span data-ttu-id="3af59-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3af59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3af59-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3af59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3af59-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3af59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3af59-107">Criar um novo objeto [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) .</span><span class="sxs-lookup"><span data-stu-id="3af59-107">Create a new [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3af59-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3af59-108">Prerequisites</span></span>
<span data-ttu-id="3af59-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3af59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3af59-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3af59-111">Permission type</span></span>|<span data-ttu-id="3af59-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3af59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3af59-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3af59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3af59-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3af59-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3af59-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3af59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3af59-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3af59-116">Not supported.</span></span>|
|<span data-ttu-id="3af59-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3af59-117">Application</span></span>|<span data-ttu-id="3af59-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3af59-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3af59-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3af59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBaselines
```

## <a name="request-headers"></a><span data-ttu-id="3af59-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3af59-120">Request headers</span></span>
|<span data-ttu-id="3af59-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3af59-121">Header</span></span>|<span data-ttu-id="3af59-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3af59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3af59-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3af59-123">Authorization</span></span>|<span data-ttu-id="3af59-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3af59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3af59-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3af59-125">Accept</span></span>|<span data-ttu-id="3af59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3af59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3af59-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3af59-127">Request body</span></span>
<span data-ttu-id="3af59-128">No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsBaseline.</span><span class="sxs-lookup"><span data-stu-id="3af59-128">In the request body, supply a JSON representation for the userExperienceAnalyticsBaseline object.</span></span>

<span data-ttu-id="3af59-129">A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsBaseline.</span><span class="sxs-lookup"><span data-stu-id="3af59-129">The following table shows the properties that are required when you create the userExperienceAnalyticsBaseline.</span></span>

|<span data-ttu-id="3af59-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3af59-130">Property</span></span>|<span data-ttu-id="3af59-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3af59-131">Type</span></span>|<span data-ttu-id="3af59-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3af59-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3af59-133">id</span><span class="sxs-lookup"><span data-stu-id="3af59-133">id</span></span>|<span data-ttu-id="3af59-134">String</span><span class="sxs-lookup"><span data-stu-id="3af59-134">String</span></span>|<span data-ttu-id="3af59-135">O identificador exclusivo da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="3af59-135">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="3af59-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3af59-136">displayName</span></span>|<span data-ttu-id="3af59-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3af59-137">String</span></span>|<span data-ttu-id="3af59-138">O nome da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="3af59-138">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="3af59-139">overallScore</span><span class="sxs-lookup"><span data-stu-id="3af59-139">overallScore</span></span>|<span data-ttu-id="3af59-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3af59-140">Int32</span></span>|<span data-ttu-id="3af59-141">A pontuação geral da linha de base da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="3af59-141">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="3af59-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="3af59-142">isBuiltIn</span></span>|<span data-ttu-id="3af59-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="3af59-143">Boolean</span></span>|<span data-ttu-id="3af59-144">Significa se a linha de base atual é a linha de base mediana comercial ou uma linha de base personalizada.</span><span class="sxs-lookup"><span data-stu-id="3af59-144">Signifies if the current baseline is the commercial median baseline or a custom baseline.</span></span>|
|<span data-ttu-id="3af59-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3af59-145">createdDateTime</span></span>|<span data-ttu-id="3af59-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3af59-146">DateTimeOffset</span></span>|<span data-ttu-id="3af59-147">A data em que a linha de base personalizada foi criada.</span><span class="sxs-lookup"><span data-stu-id="3af59-147">The date the custom baseline was created.</span></span>|



## <a name="response"></a><span data-ttu-id="3af59-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="3af59-148">Response</span></span>
<span data-ttu-id="3af59-149">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3af59-149">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3af59-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3af59-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="3af59-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3af59-151">Request</span></span>
<span data-ttu-id="3af59-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3af59-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3af59-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="3af59-153">Response</span></span>
<span data-ttu-id="3af59-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3af59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





