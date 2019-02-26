---
title: Criar embeddedSIMActivationCodePool
description: Criar um novo objeto embeddedSIMActivationCodePool.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c0cf5f48f10d01fbaf5e15d74d8fb2421e203f7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174598"
---
# <a name="create-embeddedsimactivationcodepool"></a><span data-ttu-id="0efdf-103">Criar embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="0efdf-103">Create embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="0efdf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0efdf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0efdf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0efdf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0efdf-106">Criar um novo objeto [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="0efdf-106">Create a new [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0efdf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0efdf-107">Prerequisites</span></span>
<span data-ttu-id="0efdf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0efdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0efdf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0efdf-110">Permission type</span></span>|<span data-ttu-id="0efdf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0efdf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0efdf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0efdf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0efdf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0efdf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0efdf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0efdf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0efdf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0efdf-115">Not supported.</span></span>|
|<span data-ttu-id="0efdf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0efdf-116">Application</span></span>|<span data-ttu-id="0efdf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0efdf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0efdf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0efdf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a><span data-ttu-id="0efdf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0efdf-119">Request headers</span></span>
|<span data-ttu-id="0efdf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0efdf-120">Header</span></span>|<span data-ttu-id="0efdf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0efdf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0efdf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0efdf-122">Authorization</span></span>|<span data-ttu-id="0efdf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0efdf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0efdf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0efdf-124">Accept</span></span>|<span data-ttu-id="0efdf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0efdf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0efdf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0efdf-126">Request body</span></span>
<span data-ttu-id="0efdf-127">No corpo da solicitação, forneça uma representação JSON do objeto embeddedSIMActivationCodePool.</span><span class="sxs-lookup"><span data-stu-id="0efdf-127">In the request body, supply a JSON representation for the embeddedSIMActivationCodePool object.</span></span>

<span data-ttu-id="0efdf-128">A tabela a seguir mostra as propriedades que são necessárias ao criar embeddedSIMActivationCodePool.</span><span class="sxs-lookup"><span data-stu-id="0efdf-128">The following table shows the properties that are required when you create the embeddedSIMActivationCodePool.</span></span>

|<span data-ttu-id="0efdf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0efdf-129">Property</span></span>|<span data-ttu-id="0efdf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0efdf-130">Type</span></span>|<span data-ttu-id="0efdf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0efdf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0efdf-132">id</span><span class="sxs-lookup"><span data-stu-id="0efdf-132">id</span></span>|<span data-ttu-id="0efdf-133">String</span><span class="sxs-lookup"><span data-stu-id="0efdf-133">String</span></span>|<span data-ttu-id="0efdf-134">Identificador exclusivo do pool de códigos de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="0efdf-134">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="0efdf-135">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="0efdf-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="0efdf-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0efdf-136">displayName</span></span>|<span data-ttu-id="0efdf-137">String</span><span class="sxs-lookup"><span data-stu-id="0efdf-137">String</span></span>|<span data-ttu-id="0efdf-138">O nome definido pelo administrador do pool de código de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="0efdf-138">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="0efdf-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0efdf-139">createdDateTime</span></span>|<span data-ttu-id="0efdf-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0efdf-140">DateTimeOffset</span></span>|<span data-ttu-id="0efdf-141">A hora em que o pool de códigos de ativação do SIM incorporado foi criado.</span><span class="sxs-lookup"><span data-stu-id="0efdf-141">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="0efdf-142">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="0efdf-142">Generated service side.</span></span>|
|<span data-ttu-id="0efdf-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0efdf-143">modifiedDateTime</span></span>|<span data-ttu-id="0efdf-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0efdf-144">DateTimeOffset</span></span>|<span data-ttu-id="0efdf-145">A hora em que o pool de código de ativação do SIM incorporado foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0efdf-145">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="0efdf-146">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="0efdf-146">Updated service side.</span></span>|
|<span data-ttu-id="0efdf-147">activationCodes</span><span class="sxs-lookup"><span data-stu-id="0efdf-147">activationCodes</span></span>|<span data-ttu-id="0efdf-148">coleção [embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)</span><span class="sxs-lookup"><span data-stu-id="0efdf-148">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="0efdf-149">Os códigos de ativação que pertencem a esse pool.</span><span class="sxs-lookup"><span data-stu-id="0efdf-149">The activation codes which belong to this pool.</span></span> <span data-ttu-id="0efdf-150">Essa propriedade de navegação é usada para lançar códigos de ativação no Intune, mas não pode ser usado para ler códigos de ativação do Intune.</span><span class="sxs-lookup"><span data-stu-id="0efdf-150">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="0efdf-151">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="0efdf-151">activationCodeCount</span></span>|<span data-ttu-id="0efdf-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0efdf-152">Int32</span></span>|<span data-ttu-id="0efdf-153">A contagem total de códigos de ativação que pertencem a esse pool.</span><span class="sxs-lookup"><span data-stu-id="0efdf-153">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="0efdf-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="0efdf-154">Response</span></span>
<span data-ttu-id="0efdf-155">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0efdf-155">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0efdf-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0efdf-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="0efdf-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0efdf-157">Request</span></span>
<span data-ttu-id="0efdf-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0efdf-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools
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

### <a name="response"></a><span data-ttu-id="0efdf-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="0efdf-159">Response</span></span>
<span data-ttu-id="0efdf-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0efdf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




