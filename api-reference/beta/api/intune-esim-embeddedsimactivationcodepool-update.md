---
title: Atualizar embeddedSIMActivationCodePool
description: Atualize as propriedades de um objeto EMBEDDEDSIMActivationCodePool incorporado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: be9d88f6f75d677cf3b8133e8e094da2f1c09dda
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126126"
---
# <a name="update-embeddedsimactivationcodepool"></a><span data-ttu-id="ec405-103">Atualizar embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="ec405-103">Update embeddedSIMActivationCodePool</span></span>

<span data-ttu-id="ec405-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec405-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec405-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ec405-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec405-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec405-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec405-107">Atualize as propriedades de [um objeto EMBEDDEDSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) incorporado.</span><span class="sxs-lookup"><span data-stu-id="ec405-107">Update the properties of a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec405-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ec405-108">Prerequisites</span></span>
<span data-ttu-id="ec405-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec405-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec405-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec405-111">Permission type</span></span>|<span data-ttu-id="ec405-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec405-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec405-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec405-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec405-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec405-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ec405-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec405-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec405-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec405-116">Not supported.</span></span>|
|<span data-ttu-id="ec405-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec405-117">Application</span></span>|<span data-ttu-id="ec405-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec405-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec405-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec405-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a><span data-ttu-id="ec405-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec405-120">Request headers</span></span>
|<span data-ttu-id="ec405-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec405-121">Header</span></span>|<span data-ttu-id="ec405-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ec405-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec405-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec405-123">Authorization</span></span>|<span data-ttu-id="ec405-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec405-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec405-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ec405-125">Accept</span></span>|<span data-ttu-id="ec405-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ec405-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec405-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec405-127">Request body</span></span>
<span data-ttu-id="ec405-128">No corpo da solicitação, fornece uma representação JSON para o [objeto embeddedSIMActivationCodePool.](../resources/intune-esim-embeddedsimactivationcodepool.md)</span><span class="sxs-lookup"><span data-stu-id="ec405-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

<span data-ttu-id="ec405-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span><span class="sxs-lookup"><span data-stu-id="ec405-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span></span>

|<span data-ttu-id="ec405-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec405-130">Property</span></span>|<span data-ttu-id="ec405-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec405-131">Type</span></span>|<span data-ttu-id="ec405-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec405-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec405-133">id</span><span class="sxs-lookup"><span data-stu-id="ec405-133">id</span></span>|<span data-ttu-id="ec405-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec405-134">String</span></span>|<span data-ttu-id="ec405-135">Identificador exclusivo para o pool de código de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="ec405-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="ec405-136">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="ec405-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="ec405-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ec405-137">displayName</span></span>|<span data-ttu-id="ec405-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec405-138">String</span></span>|<span data-ttu-id="ec405-139">O nome definido pelo administrador do pool de código de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="ec405-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="ec405-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ec405-140">createdDateTime</span></span>|<span data-ttu-id="ec405-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec405-141">DateTimeOffset</span></span>|<span data-ttu-id="ec405-142">A hora em que o pool de código de ativação do SIM incorporado foi criado.</span><span class="sxs-lookup"><span data-stu-id="ec405-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="ec405-143">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="ec405-143">Generated service side.</span></span>|
|<span data-ttu-id="ec405-144">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec405-144">modifiedDateTime</span></span>|<span data-ttu-id="ec405-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec405-145">DateTimeOffset</span></span>|<span data-ttu-id="ec405-146">A hora em que o pool de código de ativação do SIM incorporado foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ec405-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="ec405-147">Lado do serviço atualizado.</span><span class="sxs-lookup"><span data-stu-id="ec405-147">Updated service side.</span></span>|
|<span data-ttu-id="ec405-148">activationCodes</span><span class="sxs-lookup"><span data-stu-id="ec405-148">activationCodes</span></span>|<span data-ttu-id="ec405-149">[Coleção embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)</span><span class="sxs-lookup"><span data-stu-id="ec405-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="ec405-150">Os códigos de ativação que pertencem a esse pool.</span><span class="sxs-lookup"><span data-stu-id="ec405-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="ec405-151">Essa propriedade de navegação é usada para postar códigos de ativação no Intune, mas não pode ser usada para ler códigos de ativação do Intune.</span><span class="sxs-lookup"><span data-stu-id="ec405-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="ec405-152">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="ec405-152">activationCodeCount</span></span>|<span data-ttu-id="ec405-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ec405-153">Int32</span></span>|<span data-ttu-id="ec405-154">A contagem total de códigos de ativação que pertencem a esse pool.</span><span class="sxs-lookup"><span data-stu-id="ec405-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="ec405-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec405-155">Response</span></span>
<span data-ttu-id="ec405-156">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec405-156">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec405-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec405-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec405-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec405-158">Request</span></span>
<span data-ttu-id="ec405-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec405-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
Content-type: application/json
Content-length: 460

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "displayName": "Display Name value",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```

### <a name="response"></a><span data-ttu-id="ec405-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec405-160">Response</span></span>
<span data-ttu-id="ec405-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec405-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 628

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "ec308741-8741-ec30-4187-30ec418730ec",
  "displayName": "Display Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```




