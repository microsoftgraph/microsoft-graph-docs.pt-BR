---
title: Atualizar ndesConnector
description: Atualize as propriedades de um objeto ndesConnector.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ef3857d6b12803279c50540883125ec0685ff81b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847310"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="11559-103">Atualizar ndesConnector</span><span class="sxs-lookup"><span data-stu-id="11559-103">Update ndesConnector</span></span>

> <span data-ttu-id="11559-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="11559-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11559-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="11559-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11559-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="11559-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11559-107">Atualize as propriedades de um objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="11559-107">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="11559-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="11559-108">Prerequisites</span></span>
<span data-ttu-id="11559-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11559-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11559-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11559-111">Permission type</span></span>|<span data-ttu-id="11559-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="11559-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11559-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11559-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11559-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11559-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="11559-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11559-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11559-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11559-116">Not supported.</span></span>|
|<span data-ttu-id="11559-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11559-117">Application</span></span>|<span data-ttu-id="11559-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11559-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11559-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11559-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="11559-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11559-120">Request headers</span></span>
|<span data-ttu-id="11559-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11559-121">Header</span></span>|<span data-ttu-id="11559-122">Valor</span><span class="sxs-lookup"><span data-stu-id="11559-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11559-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="11559-123">Authorization</span></span>|<span data-ttu-id="11559-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11559-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11559-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="11559-125">Accept</span></span>|<span data-ttu-id="11559-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11559-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11559-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11559-127">Request body</span></span>
<span data-ttu-id="11559-128">No corpo da solicitação, fornece uma representação JSON para o objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="11559-128">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="11559-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span><span class="sxs-lookup"><span data-stu-id="11559-129">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="11559-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11559-130">Property</span></span>|<span data-ttu-id="11559-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="11559-131">Type</span></span>|<span data-ttu-id="11559-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="11559-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11559-133">id</span><span class="sxs-lookup"><span data-stu-id="11559-133">id</span></span>|<span data-ttu-id="11559-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11559-134">String</span></span>|<span data-ttu-id="11559-135">A chave do conector NDES.</span><span class="sxs-lookup"><span data-stu-id="11559-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="11559-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="11559-136">lastConnectionDateTime</span></span>|<span data-ttu-id="11559-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11559-137">DateTimeOffset</span></span>|<span data-ttu-id="11559-138">Hora da última conexão para o conector Ndes</span><span class="sxs-lookup"><span data-stu-id="11559-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="11559-139">estado</span><span class="sxs-lookup"><span data-stu-id="11559-139">state</span></span>|[<span data-ttu-id="11559-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="11559-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="11559-141">Status do conector NDES.</span><span class="sxs-lookup"><span data-stu-id="11559-141">Ndes Connector Status.</span></span> <span data-ttu-id="11559-142">Os valores possíveis são: `none`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="11559-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="11559-143">displayName</span><span class="sxs-lookup"><span data-stu-id="11559-143">displayName</span></span>|<span data-ttu-id="11559-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11559-144">String</span></span>|<span data-ttu-id="11559-145">O nome amigável do conector Ndes.</span><span class="sxs-lookup"><span data-stu-id="11559-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="11559-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="11559-146">Response</span></span>
<span data-ttu-id="11559-147">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11559-147">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11559-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11559-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="11559-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11559-149">Request</span></span>
<span data-ttu-id="11559-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11559-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/ndesConnectors/{ndesConnectorId}
Content-type: application/json
Content-length: 131

{
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="11559-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="11559-151">Response</span></span>
<span data-ttu-id="11559-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11559-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```





