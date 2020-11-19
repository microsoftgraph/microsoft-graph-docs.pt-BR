---
title: Atualizar defaultDeviceCompliancePolicy
description: Atualiza as propriedades de um objeto defaultDeviceCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0c3c598b984e98a1d37b5da7632c95a088def3c2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49265273"
---
# <a name="update-defaultdevicecompliancepolicy"></a><span data-ttu-id="06aab-103">Atualizar defaultDeviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="06aab-103">Update defaultDeviceCompliancePolicy</span></span>

<span data-ttu-id="06aab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06aab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06aab-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="06aab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06aab-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06aab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06aab-107">Atualiza as propriedades de um objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="06aab-107">Update the properties of a [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06aab-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06aab-108">Prerequisites</span></span>
<span data-ttu-id="06aab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06aab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06aab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06aab-111">Permission type</span></span>|<span data-ttu-id="06aab-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06aab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06aab-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06aab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06aab-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06aab-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06aab-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06aab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06aab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06aab-116">Not supported.</span></span>|
|<span data-ttu-id="06aab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06aab-117">Application</span></span>|<span data-ttu-id="06aab-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06aab-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06aab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06aab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="06aab-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06aab-120">Request headers</span></span>
|<span data-ttu-id="06aab-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06aab-121">Header</span></span>|<span data-ttu-id="06aab-122">Valor</span><span class="sxs-lookup"><span data-stu-id="06aab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06aab-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="06aab-123">Authorization</span></span>|<span data-ttu-id="06aab-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06aab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06aab-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06aab-125">Accept</span></span>|<span data-ttu-id="06aab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06aab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06aab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06aab-127">Request body</span></span>
<span data-ttu-id="06aab-128">No corpo da solicitação, forneça uma representação JSON do objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="06aab-128">In the request body, supply a JSON representation for the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object.</span></span>

<span data-ttu-id="06aab-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06aab-129">The following table shows the properties that are required when you create the [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).</span></span>

|<span data-ttu-id="06aab-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06aab-130">Property</span></span>|<span data-ttu-id="06aab-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="06aab-131">Type</span></span>|<span data-ttu-id="06aab-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="06aab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06aab-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="06aab-133">roleScopeTagIds</span></span>|<span data-ttu-id="06aab-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="06aab-134">String collection</span></span>|<span data-ttu-id="06aab-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="06aab-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="06aab-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06aab-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06aab-137">id</span><span class="sxs-lookup"><span data-stu-id="06aab-137">id</span></span>|<span data-ttu-id="06aab-138">String</span><span class="sxs-lookup"><span data-stu-id="06aab-138">String</span></span>|<span data-ttu-id="06aab-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="06aab-139">Key of the entity.</span></span> <span data-ttu-id="06aab-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06aab-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06aab-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06aab-141">createdDateTime</span></span>|<span data-ttu-id="06aab-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06aab-142">DateTimeOffset</span></span>|<span data-ttu-id="06aab-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="06aab-143">DateTime the object was created.</span></span> <span data-ttu-id="06aab-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06aab-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06aab-145">description</span><span class="sxs-lookup"><span data-stu-id="06aab-145">description</span></span>|<span data-ttu-id="06aab-146">String</span><span class="sxs-lookup"><span data-stu-id="06aab-146">String</span></span>|<span data-ttu-id="06aab-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06aab-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="06aab-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06aab-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06aab-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06aab-149">lastModifiedDateTime</span></span>|<span data-ttu-id="06aab-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06aab-150">DateTimeOffset</span></span>|<span data-ttu-id="06aab-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="06aab-151">DateTime the object was last modified.</span></span> <span data-ttu-id="06aab-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06aab-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06aab-153">displayName</span><span class="sxs-lookup"><span data-stu-id="06aab-153">displayName</span></span>|<span data-ttu-id="06aab-154">String</span><span class="sxs-lookup"><span data-stu-id="06aab-154">String</span></span>|<span data-ttu-id="06aab-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06aab-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="06aab-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06aab-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06aab-157">version</span><span class="sxs-lookup"><span data-stu-id="06aab-157">version</span></span>|<span data-ttu-id="06aab-158">Int32</span><span class="sxs-lookup"><span data-stu-id="06aab-158">Int32</span></span>|<span data-ttu-id="06aab-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06aab-159">Version of the device configuration.</span></span> <span data-ttu-id="06aab-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06aab-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|



## <a name="response"></a><span data-ttu-id="06aab-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="06aab-161">Response</span></span>
<span data-ttu-id="06aab-162">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06aab-162">If successful, this method returns a `200 OK` response code and an updated [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06aab-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06aab-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="06aab-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06aab-164">Request</span></span>
<span data-ttu-id="06aab-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06aab-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 229

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="06aab-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="06aab-166">Response</span></span>
<span data-ttu-id="06aab-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06aab-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "a285f027-f027-a285-27f0-85a227f085a2",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```




