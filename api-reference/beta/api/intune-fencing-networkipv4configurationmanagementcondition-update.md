---
title: Atualizar networkIPv4ConfigurationManagementCondition
description: Atualiza as propriedades de um objeto networkIPv4ConfigurationManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01ade0f662fc909ab8370cc17da5db239ba13893
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43384445"
---
# <a name="update-networkipv4configurationmanagementcondition"></a><span data-ttu-id="ee2a4-103">Atualizar networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="ee2a4-103">Update networkIPv4ConfigurationManagementCondition</span></span>

<span data-ttu-id="ee2a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee2a4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee2a4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee2a4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee2a4-107">Atualiza as propriedades de um objeto [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="ee2a4-107">Update the properties of a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee2a4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ee2a4-108">Prerequisites</span></span>
<span data-ttu-id="ee2a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee2a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee2a4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee2a4-111">Permission type</span></span>|<span data-ttu-id="ee2a4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ee2a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee2a4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee2a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee2a4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee2a4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee2a4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee2a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee2a4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-116">Not supported.</span></span>|
|<span data-ttu-id="ee2a4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee2a4-117">Application</span></span>|<span data-ttu-id="ee2a4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee2a4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee2a4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee2a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="ee2a4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee2a4-120">Request headers</span></span>
|<span data-ttu-id="ee2a4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ee2a4-121">Header</span></span>|<span data-ttu-id="ee2a4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ee2a4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee2a4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee2a4-123">Authorization</span></span>|<span data-ttu-id="ee2a4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee2a4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ee2a4-125">Accept</span></span>|<span data-ttu-id="ee2a4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee2a4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee2a4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee2a4-127">Request body</span></span>
<span data-ttu-id="ee2a4-128">No corpo da solicitação, forneça uma representação JSON do objeto [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="ee2a4-128">In the request body, supply a JSON representation for the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="ee2a4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="ee2a4-129">The following table shows the properties that are required when you create the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="ee2a4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee2a4-130">Property</span></span>|<span data-ttu-id="ee2a4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee2a4-131">Type</span></span>|<span data-ttu-id="ee2a4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee2a4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee2a4-133">id</span><span class="sxs-lookup"><span data-stu-id="ee2a4-133">id</span></span>|<span data-ttu-id="ee2a4-134">String</span><span class="sxs-lookup"><span data-stu-id="ee2a4-134">String</span></span>|<span data-ttu-id="ee2a4-135">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="ee2a4-136">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-136">System generated value assigned when created.</span></span> <span data-ttu-id="ee2a4-137">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ee2a4-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ee2a4-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="ee2a4-138">uniqueName</span></span>|<span data-ttu-id="ee2a4-139">String</span><span class="sxs-lookup"><span data-stu-id="ee2a4-139">String</span></span>|<span data-ttu-id="ee2a4-140">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-140">Unique name for the management condition.</span></span> <span data-ttu-id="ee2a4-141">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-141">Used in management condition expressions.</span></span> <span data-ttu-id="ee2a4-142">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ee2a4-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ee2a4-143">displayName</span><span class="sxs-lookup"><span data-stu-id="ee2a4-143">displayName</span></span>|<span data-ttu-id="ee2a4-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee2a4-144">String</span></span>|<span data-ttu-id="ee2a4-145">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="ee2a4-146">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ee2a4-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ee2a4-147">description</span><span class="sxs-lookup"><span data-stu-id="ee2a4-147">description</span></span>|<span data-ttu-id="ee2a4-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee2a4-148">String</span></span>|<span data-ttu-id="ee2a4-149">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="ee2a4-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ee2a4-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ee2a4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee2a4-151">createdDateTime</span></span>|<span data-ttu-id="ee2a4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee2a4-152">DateTimeOffset</span></span>|<span data-ttu-id="ee2a4-153">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-153">The time the management condition was created.</span></span> <span data-ttu-id="ee2a4-154">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-154">Generated service side.</span></span> <span data-ttu-id="ee2a4-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ee2a4-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ee2a4-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee2a4-156">modifiedDateTime</span></span>|<span data-ttu-id="ee2a4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee2a4-157">DateTimeOffset</span></span>|<span data-ttu-id="ee2a4-158">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-158">The time the management condition was last modified.</span></span> <span data-ttu-id="ee2a4-159">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-159">Updated service side.</span></span> <span data-ttu-id="ee2a4-160">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ee2a4-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ee2a4-161">eTag</span><span class="sxs-lookup"><span data-stu-id="ee2a4-161">eTag</span></span>|<span data-ttu-id="ee2a4-162">String</span><span class="sxs-lookup"><span data-stu-id="ee2a4-162">String</span></span>|<span data-ttu-id="ee2a4-163">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-163">ETag of the management condition.</span></span> <span data-ttu-id="ee2a4-164">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-164">Updated service side.</span></span> <span data-ttu-id="ee2a4-165">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ee2a4-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ee2a4-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="ee2a4-166">applicablePlatforms</span></span>|<span data-ttu-id="ee2a4-167">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="ee2a4-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="ee2a4-168">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="ee2a4-169">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="ee2a4-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="ee2a4-170">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="ee2a4-171">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="ee2a4-171">ipV4Prefix</span></span>|<span data-ttu-id="ee2a4-172">String</span><span class="sxs-lookup"><span data-stu-id="ee2a4-172">String</span></span>|<span data-ttu-id="ee2a4-173">A sub-rede IPv4 à qual está conectada.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-173">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="ee2a4-174">por exemplo, 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="ee2a4-174">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="ee2a4-175">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="ee2a4-175">ipV4Gateway</span></span>|<span data-ttu-id="ee2a4-176">String</span><span class="sxs-lookup"><span data-stu-id="ee2a4-176">String</span></span>|<span data-ttu-id="ee2a4-177">O endereço do gateway IPv4.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-177">The IPv4 gateway address.</span></span> <span data-ttu-id="ee2a4-178">por exemplo, 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="ee2a4-178">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="ee2a4-179">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="ee2a4-179">ipV4DHCPServer</span></span>|<span data-ttu-id="ee2a4-180">String</span><span class="sxs-lookup"><span data-stu-id="ee2a4-180">String</span></span>|<span data-ttu-id="ee2a4-181">O endereço IPv4 do servidor DHCP para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-181">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="ee2a4-182">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="ee2a4-182">ipV4DNSServerList</span></span>|<span data-ttu-id="ee2a4-183">Coleção String</span><span class="sxs-lookup"><span data-stu-id="ee2a4-183">String collection</span></span>|<span data-ttu-id="ee2a4-184">Os servidores DNS IPv4 configurados para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-184">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="ee2a4-185">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="ee2a4-185">dnsSuffixList</span></span>|<span data-ttu-id="ee2a4-186">Coleção String</span><span class="sxs-lookup"><span data-stu-id="ee2a4-186">String collection</span></span>|<span data-ttu-id="ee2a4-187">Sufixos DNS válidos para a rede atual.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-187">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="ee2a4-188">por exemplo, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="ee2a4-188">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="ee2a4-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee2a4-189">Response</span></span>
<span data-ttu-id="ee2a4-190">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-190">If successful, this method returns a `200 OK` response code and an updated [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee2a4-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee2a4-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee2a4-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee2a4-192">Request</span></span>
<span data-ttu-id="ee2a4-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 529

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="ee2a4-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee2a4-194">Response</span></span>
<span data-ttu-id="ee2a4-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee2a4-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```



