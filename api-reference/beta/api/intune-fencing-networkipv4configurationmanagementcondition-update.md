---
title: Atualizar networkIPv4ConfigurationManagementCondition
description: Atualiza as propriedades de um objeto networkIPv4ConfigurationManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bb7c70a3d86a34c8ca3ce1402370ebf7231596c9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701918"
---
# <a name="update-networkipv4configurationmanagementcondition"></a><span data-ttu-id="b2242-103">Atualizar networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="b2242-103">Update networkIPv4ConfigurationManagementCondition</span></span>

<span data-ttu-id="b2242-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2242-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2242-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2242-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2242-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2242-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2242-107">Atualiza as propriedades de um objeto [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="b2242-107">Update the properties of a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2242-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2242-108">Prerequisites</span></span>
<span data-ttu-id="b2242-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2242-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2242-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2242-111">Permission type</span></span>|<span data-ttu-id="b2242-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2242-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2242-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2242-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2242-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2242-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2242-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2242-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2242-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2242-116">Not supported.</span></span>|
|<span data-ttu-id="b2242-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2242-117">Application</span></span>|<span data-ttu-id="b2242-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2242-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2242-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2242-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="b2242-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2242-120">Request headers</span></span>
|<span data-ttu-id="b2242-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2242-121">Header</span></span>|<span data-ttu-id="b2242-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b2242-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2242-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2242-123">Authorization</span></span>|<span data-ttu-id="b2242-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2242-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2242-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2242-125">Accept</span></span>|<span data-ttu-id="b2242-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2242-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2242-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2242-127">Request body</span></span>
<span data-ttu-id="b2242-128">No corpo da solicitação, forneça uma representação JSON do objeto [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="b2242-128">In the request body, supply a JSON representation for the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="b2242-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="b2242-129">The following table shows the properties that are required when you create the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="b2242-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2242-130">Property</span></span>|<span data-ttu-id="b2242-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2242-131">Type</span></span>|<span data-ttu-id="b2242-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2242-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2242-133">id</span><span class="sxs-lookup"><span data-stu-id="b2242-133">id</span></span>|<span data-ttu-id="b2242-134">String</span><span class="sxs-lookup"><span data-stu-id="b2242-134">String</span></span>|<span data-ttu-id="b2242-135">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b2242-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="b2242-136">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="b2242-136">System generated value assigned when created.</span></span> <span data-ttu-id="b2242-137">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b2242-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b2242-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="b2242-138">uniqueName</span></span>|<span data-ttu-id="b2242-139">String</span><span class="sxs-lookup"><span data-stu-id="b2242-139">String</span></span>|<span data-ttu-id="b2242-140">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b2242-140">Unique name for the management condition.</span></span> <span data-ttu-id="b2242-141">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b2242-141">Used in management condition expressions.</span></span> <span data-ttu-id="b2242-142">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b2242-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b2242-143">displayName</span><span class="sxs-lookup"><span data-stu-id="b2242-143">displayName</span></span>|<span data-ttu-id="b2242-144">String</span><span class="sxs-lookup"><span data-stu-id="b2242-144">String</span></span>|<span data-ttu-id="b2242-145">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b2242-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="b2242-146">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b2242-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b2242-147">description</span><span class="sxs-lookup"><span data-stu-id="b2242-147">description</span></span>|<span data-ttu-id="b2242-148">String</span><span class="sxs-lookup"><span data-stu-id="b2242-148">String</span></span>|<span data-ttu-id="b2242-149">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b2242-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="b2242-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b2242-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b2242-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2242-151">createdDateTime</span></span>|<span data-ttu-id="b2242-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2242-152">DateTimeOffset</span></span>|<span data-ttu-id="b2242-153">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="b2242-153">The time the management condition was created.</span></span> <span data-ttu-id="b2242-154">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="b2242-154">Generated service side.</span></span> <span data-ttu-id="b2242-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b2242-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b2242-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2242-156">modifiedDateTime</span></span>|<span data-ttu-id="b2242-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2242-157">DateTimeOffset</span></span>|<span data-ttu-id="b2242-158">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b2242-158">The time the management condition was last modified.</span></span> <span data-ttu-id="b2242-159">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="b2242-159">Updated service side.</span></span> <span data-ttu-id="b2242-160">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b2242-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b2242-161">eTag</span><span class="sxs-lookup"><span data-stu-id="b2242-161">eTag</span></span>|<span data-ttu-id="b2242-162">String</span><span class="sxs-lookup"><span data-stu-id="b2242-162">String</span></span>|<span data-ttu-id="b2242-163">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b2242-163">ETag of the management condition.</span></span> <span data-ttu-id="b2242-164">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="b2242-164">Updated service side.</span></span> <span data-ttu-id="b2242-165">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b2242-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b2242-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="b2242-166">applicablePlatforms</span></span>|<span data-ttu-id="b2242-167">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="b2242-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="b2242-168">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b2242-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="b2242-169">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="b2242-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="b2242-170">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b2242-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="b2242-171">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="b2242-171">ipV4Prefix</span></span>|<span data-ttu-id="b2242-172">String</span><span class="sxs-lookup"><span data-stu-id="b2242-172">String</span></span>|<span data-ttu-id="b2242-173">A sub-rede IPv4 à qual está conectada.</span><span class="sxs-lookup"><span data-stu-id="b2242-173">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="b2242-174">por exemplo, 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="b2242-174">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="b2242-175">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="b2242-175">ipV4Gateway</span></span>|<span data-ttu-id="b2242-176">String</span><span class="sxs-lookup"><span data-stu-id="b2242-176">String</span></span>|<span data-ttu-id="b2242-177">O endereço do gateway IPv4.</span><span class="sxs-lookup"><span data-stu-id="b2242-177">The IPv4 gateway address.</span></span> <span data-ttu-id="b2242-178">por exemplo, 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="b2242-178">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="b2242-179">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="b2242-179">ipV4DHCPServer</span></span>|<span data-ttu-id="b2242-180">String</span><span class="sxs-lookup"><span data-stu-id="b2242-180">String</span></span>|<span data-ttu-id="b2242-181">O endereço IPv4 do servidor DHCP para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="b2242-181">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="b2242-182">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="b2242-182">ipV4DNSServerList</span></span>|<span data-ttu-id="b2242-183">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2242-183">String collection</span></span>|<span data-ttu-id="b2242-184">Os servidores DNS IPv4 configurados para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="b2242-184">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="b2242-185">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="b2242-185">dnsSuffixList</span></span>|<span data-ttu-id="b2242-186">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2242-186">String collection</span></span>|<span data-ttu-id="b2242-187">Sufixos DNS válidos para a rede atual.</span><span class="sxs-lookup"><span data-stu-id="b2242-187">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="b2242-188">por exemplo, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="b2242-188">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="b2242-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2242-189">Response</span></span>
<span data-ttu-id="b2242-190">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2242-190">If successful, this method returns a `200 OK` response code and an updated [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2242-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2242-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2242-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2242-192">Request</span></span>
<span data-ttu-id="b2242-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2242-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b2242-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2242-194">Response</span></span>
<span data-ttu-id="b2242-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2242-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





