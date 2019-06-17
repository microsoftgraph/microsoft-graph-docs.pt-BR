---
title: Criar networkIPv6ConfigurationManagementCondition
description: Criar um novo objeto networkIPv6ConfigurationManagementCondition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec676bc579644e0328610a42dc172b96c5ee8036
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984362"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="e56a5-103">Criar networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="e56a5-103">Create networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="e56a5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e56a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e56a5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e56a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e56a5-106">Criar um novo objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="e56a5-106">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e56a5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e56a5-107">Prerequisites</span></span>
<span data-ttu-id="e56a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e56a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e56a5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e56a5-110">Permission type</span></span>|<span data-ttu-id="e56a5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e56a5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e56a5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e56a5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e56a5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e56a5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e56a5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e56a5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e56a5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e56a5-115">Not supported.</span></span>|
|<span data-ttu-id="e56a5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e56a5-116">Application</span></span>|<span data-ttu-id="e56a5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e56a5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e56a5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e56a5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="e56a5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e56a5-119">Request headers</span></span>
|<span data-ttu-id="e56a5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e56a5-120">Header</span></span>|<span data-ttu-id="e56a5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e56a5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e56a5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e56a5-122">Authorization</span></span>|<span data-ttu-id="e56a5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e56a5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e56a5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e56a5-124">Accept</span></span>|<span data-ttu-id="e56a5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e56a5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e56a5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e56a5-126">Request body</span></span>
<span data-ttu-id="e56a5-127">No corpo da solicitação, forneça uma representação JSON do objeto networkIPv6ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="e56a5-127">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="e56a5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar networkIPv6ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="e56a5-128">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="e56a5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e56a5-129">Property</span></span>|<span data-ttu-id="e56a5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e56a5-130">Type</span></span>|<span data-ttu-id="e56a5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e56a5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e56a5-132">id</span><span class="sxs-lookup"><span data-stu-id="e56a5-132">id</span></span>|<span data-ttu-id="e56a5-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e56a5-133">String</span></span>|<span data-ttu-id="e56a5-134">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e56a5-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="e56a5-135">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="e56a5-135">System generated value assigned when created.</span></span> <span data-ttu-id="e56a5-136">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e56a5-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e56a5-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="e56a5-137">uniqueName</span></span>|<span data-ttu-id="e56a5-138">String</span><span class="sxs-lookup"><span data-stu-id="e56a5-138">String</span></span>|<span data-ttu-id="e56a5-139">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e56a5-139">Unique name for the management condition.</span></span> <span data-ttu-id="e56a5-140">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e56a5-140">Used in management condition expressions.</span></span> <span data-ttu-id="e56a5-141">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e56a5-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e56a5-142">displayName</span><span class="sxs-lookup"><span data-stu-id="e56a5-142">displayName</span></span>|<span data-ttu-id="e56a5-143">String</span><span class="sxs-lookup"><span data-stu-id="e56a5-143">String</span></span>|<span data-ttu-id="e56a5-144">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e56a5-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="e56a5-145">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e56a5-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e56a5-146">descrição</span><span class="sxs-lookup"><span data-stu-id="e56a5-146">description</span></span>|<span data-ttu-id="e56a5-147">String</span><span class="sxs-lookup"><span data-stu-id="e56a5-147">String</span></span>|<span data-ttu-id="e56a5-148">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e56a5-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="e56a5-149">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e56a5-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e56a5-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e56a5-150">createdDateTime</span></span>|<span data-ttu-id="e56a5-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e56a5-151">DateTimeOffset</span></span>|<span data-ttu-id="e56a5-152">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="e56a5-152">The time the management condition was created.</span></span> <span data-ttu-id="e56a5-153">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="e56a5-153">Generated service side.</span></span> <span data-ttu-id="e56a5-154">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e56a5-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e56a5-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e56a5-155">modifiedDateTime</span></span>|<span data-ttu-id="e56a5-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e56a5-156">DateTimeOffset</span></span>|<span data-ttu-id="e56a5-157">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e56a5-157">The time the management condition was last modified.</span></span> <span data-ttu-id="e56a5-158">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="e56a5-158">Updated service side.</span></span> <span data-ttu-id="e56a5-159">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e56a5-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e56a5-160">eTag</span><span class="sxs-lookup"><span data-stu-id="e56a5-160">eTag</span></span>|<span data-ttu-id="e56a5-161">String</span><span class="sxs-lookup"><span data-stu-id="e56a5-161">String</span></span>|<span data-ttu-id="e56a5-162">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e56a5-162">ETag of the management condition.</span></span> <span data-ttu-id="e56a5-163">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="e56a5-163">Updated service side.</span></span> <span data-ttu-id="e56a5-164">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e56a5-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e56a5-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="e56a5-165">applicablePlatforms</span></span>|<span data-ttu-id="e56a5-166">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="e56a5-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="e56a5-167">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e56a5-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="e56a5-168">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="e56a5-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="e56a5-169">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="e56a5-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="e56a5-170">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="e56a5-170">ipV6Prefix</span></span>|<span data-ttu-id="e56a5-171">String</span><span class="sxs-lookup"><span data-stu-id="e56a5-171">String</span></span>|<span data-ttu-id="e56a5-172">A sub-rede IPv6 a ser conectada.</span><span class="sxs-lookup"><span data-stu-id="e56a5-172">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="e56a5-173">por exemplo, 2001: DB8::/32</span><span class="sxs-lookup"><span data-stu-id="e56a5-173">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="e56a5-174">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="e56a5-174">ipV6Gateway</span></span>|<span data-ttu-id="e56a5-175">String</span><span class="sxs-lookup"><span data-stu-id="e56a5-175">String</span></span>|<span data-ttu-id="e56a5-176">O endereço do gateway IPv6 para.</span><span class="sxs-lookup"><span data-stu-id="e56a5-176">The IPv6 gateway address to.</span></span> <span data-ttu-id="e56a5-177">por exemplo, 2001: DB8:: 1</span><span class="sxs-lookup"><span data-stu-id="e56a5-177">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="e56a5-178">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="e56a5-178">ipV6DNSServerList</span></span>|<span data-ttu-id="e56a5-179">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e56a5-179">String collection</span></span>|<span data-ttu-id="e56a5-180">Servidores DNS IPv6 configurados para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="e56a5-180">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="e56a5-181">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="e56a5-181">dnsSuffixList</span></span>|<span data-ttu-id="e56a5-182">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e56a5-182">String collection</span></span>|<span data-ttu-id="e56a5-183">Sufixos DNS válidos para a rede atual.</span><span class="sxs-lookup"><span data-stu-id="e56a5-183">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="e56a5-184">por exemplo, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="e56a5-184">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="e56a5-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="e56a5-185">Response</span></span>
<span data-ttu-id="e56a5-186">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e56a5-186">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e56a5-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e56a5-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="e56a5-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e56a5-188">Request</span></span>
<span data-ttu-id="e56a5-189">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e56a5-189">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e56a5-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="e56a5-190">Response</span></span>
<span data-ttu-id="e56a5-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e56a5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





