---
title: Atualizar networkIPv6ConfigurationManagementCondition
description: Atualiza as propriedades de um objeto networkIPv6ConfigurationManagementCondition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e2e6c6f7a51945e8cc54c9c80e47ea26337b4ac6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979841"
---
# <a name="update-networkipv6configurationmanagementcondition"></a><span data-ttu-id="9ad2e-103">Atualizar networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="9ad2e-103">Update networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="9ad2e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ad2e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ad2e-106">Atualiza as propriedades de um objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="9ad2e-106">Update the properties of a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ad2e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ad2e-107">Prerequisites</span></span>
<span data-ttu-id="9ad2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ad2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ad2e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ad2e-110">Permission type</span></span>|<span data-ttu-id="9ad2e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9ad2e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ad2e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ad2e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ad2e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ad2e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ad2e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ad2e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ad2e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-115">Not supported.</span></span>|
|<span data-ttu-id="9ad2e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ad2e-116">Application</span></span>|<span data-ttu-id="9ad2e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ad2e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ad2e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="9ad2e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ad2e-119">Request headers</span></span>
|<span data-ttu-id="9ad2e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ad2e-120">Header</span></span>|<span data-ttu-id="9ad2e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9ad2e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ad2e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ad2e-122">Authorization</span></span>|<span data-ttu-id="9ad2e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ad2e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9ad2e-124">Accept</span></span>|<span data-ttu-id="9ad2e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9ad2e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ad2e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ad2e-126">Request body</span></span>
<span data-ttu-id="9ad2e-127">No corpo da solicitação, forneça uma representação JSON do objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="9ad2e-127">In the request body, supply a JSON representation for the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="9ad2e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="9ad2e-128">The following table shows the properties that are required when you create the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="9ad2e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ad2e-129">Property</span></span>|<span data-ttu-id="9ad2e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ad2e-130">Type</span></span>|<span data-ttu-id="9ad2e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ad2e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ad2e-132">id</span><span class="sxs-lookup"><span data-stu-id="9ad2e-132">id</span></span>|<span data-ttu-id="9ad2e-133">String</span><span class="sxs-lookup"><span data-stu-id="9ad2e-133">String</span></span>|<span data-ttu-id="9ad2e-134">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="9ad2e-135">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-135">System generated value assigned when created.</span></span> <span data-ttu-id="9ad2e-136">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9ad2e-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9ad2e-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="9ad2e-137">uniqueName</span></span>|<span data-ttu-id="9ad2e-138">String</span><span class="sxs-lookup"><span data-stu-id="9ad2e-138">String</span></span>|<span data-ttu-id="9ad2e-139">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-139">Unique name for the management condition.</span></span> <span data-ttu-id="9ad2e-140">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-140">Used in management condition expressions.</span></span> <span data-ttu-id="9ad2e-141">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9ad2e-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9ad2e-142">displayName</span><span class="sxs-lookup"><span data-stu-id="9ad2e-142">displayName</span></span>|<span data-ttu-id="9ad2e-143">String</span><span class="sxs-lookup"><span data-stu-id="9ad2e-143">String</span></span>|<span data-ttu-id="9ad2e-144">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="9ad2e-145">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9ad2e-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9ad2e-146">descrição</span><span class="sxs-lookup"><span data-stu-id="9ad2e-146">description</span></span>|<span data-ttu-id="9ad2e-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ad2e-147">String</span></span>|<span data-ttu-id="9ad2e-148">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="9ad2e-149">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9ad2e-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9ad2e-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ad2e-150">createdDateTime</span></span>|<span data-ttu-id="9ad2e-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ad2e-151">DateTimeOffset</span></span>|<span data-ttu-id="9ad2e-152">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-152">The time the management condition was created.</span></span> <span data-ttu-id="9ad2e-153">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-153">Generated service side.</span></span> <span data-ttu-id="9ad2e-154">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9ad2e-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9ad2e-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ad2e-155">modifiedDateTime</span></span>|<span data-ttu-id="9ad2e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ad2e-156">DateTimeOffset</span></span>|<span data-ttu-id="9ad2e-157">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-157">The time the management condition was last modified.</span></span> <span data-ttu-id="9ad2e-158">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-158">Updated service side.</span></span> <span data-ttu-id="9ad2e-159">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9ad2e-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9ad2e-160">eTag</span><span class="sxs-lookup"><span data-stu-id="9ad2e-160">eTag</span></span>|<span data-ttu-id="9ad2e-161">String</span><span class="sxs-lookup"><span data-stu-id="9ad2e-161">String</span></span>|<span data-ttu-id="9ad2e-162">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-162">ETag of the management condition.</span></span> <span data-ttu-id="9ad2e-163">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-163">Updated service side.</span></span> <span data-ttu-id="9ad2e-164">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9ad2e-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9ad2e-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="9ad2e-165">applicablePlatforms</span></span>|<span data-ttu-id="9ad2e-166">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="9ad2e-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="9ad2e-167">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="9ad2e-168">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="9ad2e-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="9ad2e-169">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="9ad2e-170">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="9ad2e-170">ipV6Prefix</span></span>|<span data-ttu-id="9ad2e-171">String</span><span class="sxs-lookup"><span data-stu-id="9ad2e-171">String</span></span>|<span data-ttu-id="9ad2e-172">A sub-rede IPv6 a ser conectada.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-172">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="9ad2e-173">por exemplo, 2001: DB8::/32</span><span class="sxs-lookup"><span data-stu-id="9ad2e-173">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="9ad2e-174">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="9ad2e-174">ipV6Gateway</span></span>|<span data-ttu-id="9ad2e-175">String</span><span class="sxs-lookup"><span data-stu-id="9ad2e-175">String</span></span>|<span data-ttu-id="9ad2e-176">O endereço do gateway IPv6 para.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-176">The IPv6 gateway address to.</span></span> <span data-ttu-id="9ad2e-177">por exemplo, 2001: DB8:: 1</span><span class="sxs-lookup"><span data-stu-id="9ad2e-177">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="9ad2e-178">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="9ad2e-178">ipV6DNSServerList</span></span>|<span data-ttu-id="9ad2e-179">Coleção String</span><span class="sxs-lookup"><span data-stu-id="9ad2e-179">String collection</span></span>|<span data-ttu-id="9ad2e-180">Servidores DNS IPv6 configurados para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-180">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="9ad2e-181">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="9ad2e-181">dnsSuffixList</span></span>|<span data-ttu-id="9ad2e-182">Coleção String</span><span class="sxs-lookup"><span data-stu-id="9ad2e-182">String collection</span></span>|<span data-ttu-id="9ad2e-183">Sufixos DNS válidos para a rede atual.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-183">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="9ad2e-184">por exemplo, Seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="9ad2e-184">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="9ad2e-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ad2e-185">Response</span></span>
<span data-ttu-id="9ad2e-186">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-186">If successful, this method returns a `200 OK` response code and an updated [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ad2e-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ad2e-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ad2e-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ad2e-188">Request</span></span>
<span data-ttu-id="9ad2e-189">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
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

### <a name="response"></a><span data-ttu-id="9ad2e-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ad2e-190">Response</span></span>
<span data-ttu-id="9ad2e-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ad2e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




