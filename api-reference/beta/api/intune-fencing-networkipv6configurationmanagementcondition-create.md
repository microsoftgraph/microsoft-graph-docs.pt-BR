---
title: Criar networkIPv6ConfigurationManagementCondition
description: Criar um novo objeto networkIPv6ConfigurationManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a3fec737657928d92f1c3ff2975e2b1a0922c7d7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969981"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="10db9-103">Criar networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="10db9-103">Create networkIPv6ConfigurationManagementCondition</span></span>

<span data-ttu-id="10db9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10db9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10db9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="10db9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10db9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10db9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10db9-107">Criar um novo objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="10db9-107">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10db9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="10db9-108">Prerequisites</span></span>
<span data-ttu-id="10db9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10db9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10db9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10db9-111">Permission type</span></span>|<span data-ttu-id="10db9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="10db9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10db9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10db9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10db9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10db9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="10db9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10db9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10db9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10db9-116">Not supported.</span></span>|
|<span data-ttu-id="10db9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10db9-117">Application</span></span>|<span data-ttu-id="10db9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10db9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10db9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10db9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="10db9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10db9-120">Request headers</span></span>
|<span data-ttu-id="10db9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="10db9-121">Header</span></span>|<span data-ttu-id="10db9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="10db9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10db9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="10db9-123">Authorization</span></span>|<span data-ttu-id="10db9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10db9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10db9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="10db9-125">Accept</span></span>|<span data-ttu-id="10db9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10db9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10db9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10db9-127">Request body</span></span>
<span data-ttu-id="10db9-128">No corpo da solicitação, forneça uma representação JSON do objeto networkIPv6ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="10db9-128">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="10db9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar networkIPv6ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="10db9-129">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="10db9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10db9-130">Property</span></span>|<span data-ttu-id="10db9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="10db9-131">Type</span></span>|<span data-ttu-id="10db9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="10db9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10db9-133">id</span><span class="sxs-lookup"><span data-stu-id="10db9-133">id</span></span>|<span data-ttu-id="10db9-134">String</span><span class="sxs-lookup"><span data-stu-id="10db9-134">String</span></span>|<span data-ttu-id="10db9-135">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="10db9-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="10db9-136">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="10db9-136">System generated value assigned when created.</span></span> <span data-ttu-id="10db9-137">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="10db9-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="10db9-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="10db9-138">uniqueName</span></span>|<span data-ttu-id="10db9-139">String</span><span class="sxs-lookup"><span data-stu-id="10db9-139">String</span></span>|<span data-ttu-id="10db9-140">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="10db9-140">Unique name for the management condition.</span></span> <span data-ttu-id="10db9-141">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="10db9-141">Used in management condition expressions.</span></span> <span data-ttu-id="10db9-142">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="10db9-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="10db9-143">displayName</span><span class="sxs-lookup"><span data-stu-id="10db9-143">displayName</span></span>|<span data-ttu-id="10db9-144">String</span><span class="sxs-lookup"><span data-stu-id="10db9-144">String</span></span>|<span data-ttu-id="10db9-145">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="10db9-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="10db9-146">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="10db9-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="10db9-147">description</span><span class="sxs-lookup"><span data-stu-id="10db9-147">description</span></span>|<span data-ttu-id="10db9-148">String</span><span class="sxs-lookup"><span data-stu-id="10db9-148">String</span></span>|<span data-ttu-id="10db9-149">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="10db9-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="10db9-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="10db9-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="10db9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10db9-151">createdDateTime</span></span>|<span data-ttu-id="10db9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10db9-152">DateTimeOffset</span></span>|<span data-ttu-id="10db9-153">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="10db9-153">The time the management condition was created.</span></span> <span data-ttu-id="10db9-154">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="10db9-154">Generated service side.</span></span> <span data-ttu-id="10db9-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="10db9-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="10db9-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10db9-156">modifiedDateTime</span></span>|<span data-ttu-id="10db9-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10db9-157">DateTimeOffset</span></span>|<span data-ttu-id="10db9-158">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="10db9-158">The time the management condition was last modified.</span></span> <span data-ttu-id="10db9-159">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="10db9-159">Updated service side.</span></span> <span data-ttu-id="10db9-160">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="10db9-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="10db9-161">eTag</span><span class="sxs-lookup"><span data-stu-id="10db9-161">eTag</span></span>|<span data-ttu-id="10db9-162">String</span><span class="sxs-lookup"><span data-stu-id="10db9-162">String</span></span>|<span data-ttu-id="10db9-163">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="10db9-163">ETag of the management condition.</span></span> <span data-ttu-id="10db9-164">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="10db9-164">Updated service side.</span></span> <span data-ttu-id="10db9-165">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="10db9-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="10db9-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="10db9-166">applicablePlatforms</span></span>|<span data-ttu-id="10db9-167">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="10db9-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="10db9-168">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="10db9-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="10db9-169">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="10db9-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="10db9-170">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="10db9-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="10db9-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="10db9-171">ipV6Prefix</span></span>|<span data-ttu-id="10db9-172">String</span><span class="sxs-lookup"><span data-stu-id="10db9-172">String</span></span>|<span data-ttu-id="10db9-173">A sub-rede IPv6 a ser conectada.</span><span class="sxs-lookup"><span data-stu-id="10db9-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="10db9-174">por exemplo, 2001: DB8::/32</span><span class="sxs-lookup"><span data-stu-id="10db9-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="10db9-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="10db9-175">ipV6Gateway</span></span>|<span data-ttu-id="10db9-176">String</span><span class="sxs-lookup"><span data-stu-id="10db9-176">String</span></span>|<span data-ttu-id="10db9-177">O endereço do gateway IPv6 para.</span><span class="sxs-lookup"><span data-stu-id="10db9-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="10db9-178">por exemplo, 2001: DB8:: 1</span><span class="sxs-lookup"><span data-stu-id="10db9-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="10db9-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="10db9-179">ipV6DNSServerList</span></span>|<span data-ttu-id="10db9-180">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="10db9-180">String collection</span></span>|<span data-ttu-id="10db9-181">Servidores DNS IPv6 configurados para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="10db9-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="10db9-182">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="10db9-182">dnsSuffixList</span></span>|<span data-ttu-id="10db9-183">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="10db9-183">String collection</span></span>|<span data-ttu-id="10db9-184">Sufixos DNS válidos para a rede atual.</span><span class="sxs-lookup"><span data-stu-id="10db9-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="10db9-185">por exemplo, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="10db9-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="10db9-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="10db9-186">Response</span></span>
<span data-ttu-id="10db9-187">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10db9-187">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10db9-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10db9-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="10db9-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10db9-189">Request</span></span>
<span data-ttu-id="10db9-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10db9-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="10db9-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="10db9-191">Response</span></span>
<span data-ttu-id="10db9-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10db9-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "25811206-1206-2581-0612-812506128125",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```






