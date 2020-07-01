---
title: 'impressora: criar'
description: Cria (registra) uma impressora com o serviço de impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 1b36a856a73d78b479270138868285a852d6d187
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007133"
---
# <a name="printer-create"></a><span data-ttu-id="7f0a0-103">impressora: criar</span><span class="sxs-lookup"><span data-stu-id="7f0a0-103">printer: create</span></span>

<span data-ttu-id="7f0a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f0a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f0a0-105">Criar (registrar) uma impressora com o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-105">Create (register) a printer with the Universal Print service.</span></span> <span data-ttu-id="7f0a0-106">Esta é uma operação de execução demorada e, como tal, retorna um [printerCreateOperation](../resources/printercreateoperation.md) que pode ser usado para rastrear e verificar o registro da impressora.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-106">This is a long-running operation and as such, it returns a [printerCreateOperation](../resources/printercreateoperation.md) that can be used to track and verify the registration of the printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f0a0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f0a0-107">Permissions</span></span>
<span data-ttu-id="7f0a0-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7f0a0-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f0a0-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7f0a0-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="7f0a0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f0a0-111">Permission type</span></span> | <span data-ttu-id="7f0a0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f0a0-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7f0a0-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f0a0-113">Delegated (work or school account)</span></span>| <span data-ttu-id="7f0a0-114">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f0a0-114">User.Read.All</span></span> |
|<span data-ttu-id="7f0a0-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f0a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f0a0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-116">Not Supported.</span></span>|
|<span data-ttu-id="7f0a0-117">Application</span><span class="sxs-lookup"><span data-stu-id="7f0a0-117">Application</span></span>|<span data-ttu-id="7f0a0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f0a0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f0a0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/create
```
## <a name="request-headers"></a><span data-ttu-id="7f0a0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f0a0-120">Request headers</span></span>
| <span data-ttu-id="7f0a0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7f0a0-121">Name</span></span>       | <span data-ttu-id="7f0a0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f0a0-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7f0a0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f0a0-123">Authorization</span></span> | <span data-ttu-id="7f0a0-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-124">Bearer {token}.</span></span> <span data-ttu-id="7f0a0-125">Required.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-125">Required.</span></span> |
| <span data-ttu-id="7f0a0-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="7f0a0-126">Content-type</span></span>  | <span data-ttu-id="7f0a0-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-127">application/json.</span></span> <span data-ttu-id="7f0a0-128">Required.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f0a0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f0a0-129">Request body</span></span>
<span data-ttu-id="7f0a0-130">No corpo da solicitação, forneça um objeto JSON com as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-130">In the request body, provide a JSON object with the following properties.</span></span>

| <span data-ttu-id="7f0a0-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7f0a0-131">Parameter</span></span>      | <span data-ttu-id="7f0a0-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f0a0-132">Type</span></span>    |<span data-ttu-id="7f0a0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f0a0-133">Description</span></span>| <span data-ttu-id="7f0a0-134">Obrigatório?</span><span class="sxs-lookup"><span data-stu-id="7f0a0-134">Required?</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="7f0a0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7f0a0-135">displayName</span></span>|<span data-ttu-id="7f0a0-136">String</span><span class="sxs-lookup"><span data-stu-id="7f0a0-136">String</span></span>|<span data-ttu-id="7f0a0-137">O nome de exibição a ser atribuído à impressora.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-137">The display name to assign to the printer.</span></span>|<span data-ttu-id="7f0a0-138">Sim</span><span class="sxs-lookup"><span data-stu-id="7f0a0-138">Yes</span></span>|
|<span data-ttu-id="7f0a0-139">fabricante</span><span class="sxs-lookup"><span data-stu-id="7f0a0-139">manufacturer</span></span>|<span data-ttu-id="7f0a0-140">String</span><span class="sxs-lookup"><span data-stu-id="7f0a0-140">String</span></span>|<span data-ttu-id="7f0a0-141">O fabricante da impressora.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-141">The manufacturer of the printer.</span></span>|<span data-ttu-id="7f0a0-142">Sim</span><span class="sxs-lookup"><span data-stu-id="7f0a0-142">Yes</span></span>|
|<span data-ttu-id="7f0a0-143">modelo</span><span class="sxs-lookup"><span data-stu-id="7f0a0-143">model</span></span>|<span data-ttu-id="7f0a0-144">String</span><span class="sxs-lookup"><span data-stu-id="7f0a0-144">String</span></span>|<span data-ttu-id="7f0a0-145">O modelo da impressora.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-145">The model of the printer.</span></span>|<span data-ttu-id="7f0a0-146">Sim</span><span class="sxs-lookup"><span data-stu-id="7f0a0-146">Yes</span></span>|
|<span data-ttu-id="7f0a0-147">physicalDeviceId</span><span class="sxs-lookup"><span data-stu-id="7f0a0-147">physicalDeviceId</span></span>|<span data-ttu-id="7f0a0-148">String</span><span class="sxs-lookup"><span data-stu-id="7f0a0-148">String</span></span>|<span data-ttu-id="7f0a0-149">O UUID do dispositivo físico da impressora.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-149">The physical device UUID of the printer.</span></span> <span data-ttu-id="7f0a0-150">Obrigatório se a `hasPhysicalDevice` propriedade for true.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-150">Required if the `hasPhysicalDevice` property is true.</span></span>|<span data-ttu-id="7f0a0-151">Não</span><span class="sxs-lookup"><span data-stu-id="7f0a0-151">No</span></span>|
|<span data-ttu-id="7f0a0-152">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="7f0a0-152">hasPhysicalDevice</span></span>|<span data-ttu-id="7f0a0-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="7f0a0-153">Boolean</span></span>|<span data-ttu-id="7f0a0-154">True se a impressora tem dispositivo de saída físico; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-154">True if the printer has physical output device, false otherwise.</span></span> <span data-ttu-id="7f0a0-155">Se for omitido, o valor padrão será true.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-155">If omitted, the default value is true.</span></span>|<span data-ttu-id="7f0a0-156">Não</span><span class="sxs-lookup"><span data-stu-id="7f0a0-156">No</span></span>|
|<span data-ttu-id="7f0a0-157">certificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="7f0a0-157">certificateSigningRequest</span></span>|[<span data-ttu-id="7f0a0-158">printCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="7f0a0-158">printCertificateSigningRequest</span></span>](../resources/printcertificatesigningrequest.md)|<span data-ttu-id="7f0a0-159">A solicitação de assinatura de certificado (CSR) do X. 509 para o certificado criado e usado pela impressora para identificar-se.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-159">The X.509 Certificate Signing Request (CSR) for the certificate created and used by the printer to identify itself.</span></span>|<span data-ttu-id="7f0a0-160">Sim</span><span class="sxs-lookup"><span data-stu-id="7f0a0-160">Yes</span></span>|
|<span data-ttu-id="7f0a0-161">connectorid</span><span class="sxs-lookup"><span data-stu-id="7f0a0-161">connectorId</span></span>|<span data-ttu-id="7f0a0-162">String</span><span class="sxs-lookup"><span data-stu-id="7f0a0-162">String</span></span>|<span data-ttu-id="7f0a0-163">ID do conector que atua como proxy para a impressora.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-163">Id of Connector acting as proxy to the printer.</span></span>|<span data-ttu-id="7f0a0-164">Não</span><span class="sxs-lookup"><span data-stu-id="7f0a0-164">No</span></span>|

## <a name="response"></a><span data-ttu-id="7f0a0-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f0a0-165">Response</span></span>
<span data-ttu-id="7f0a0-166">Se tiver êxito, este método retornará um `202 Accepted` código de resposta e um link para o [printerCreateOperation](../resources/printercreateoperation.md) associado no `Operation-Location` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-166">If successful, this method returns a `202 Accepted` response code and a link to the associated [printerCreateOperation](../resources/printercreateoperation.md) in the `Operation-Location` header.</span></span>

<span data-ttu-id="7f0a0-167">Fazer uma solicitação GET para a URL vinculada pode ser usado para obter o status de um registro de impressora em andamento.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-167">Making a GET request to the linked URL can be used to get the status of an ongoing printer registration.</span></span> <span data-ttu-id="7f0a0-168">Após o registro da impressora ter sido concluído com êxito, uma solicitação GET para a URL vinculada conterá o objeto Printer criado e o certificado registrado.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-168">Once printer registration has completed successfully, a GET request to the linked URL will contain the created printer object and registered certificate.</span></span>

## <a name="example"></a><span data-ttu-id="7f0a0-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f0a0-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f0a0-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f0a0-170">Request</span></span>
<span data-ttu-id="7f0a0-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-171">The following is an example of the request.</span></span> <span data-ttu-id="7f0a0-172">Para obter ajuda para criar a solicitação de assinatura de certificado (CSR) necessária, consulte o [exemplo de código de geração de CSR](https://docs.microsoft.com/universal-print/hardware/universal-print-oem-certificate-signing-request).</span><span class="sxs-lookup"><span data-stu-id="7f0a0-172">For help creating the required Certificate Signing Request (CSR), see the [CSR generation code sample](https://docs.microsoft.com/universal-print/hardware/universal-print-oem-certificate-signing-request).</span></span>

<!-- {
  "blockType": "request",
  "name": "create_printer"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/create
Content-type: application/json
Content-length: 319

{
  "displayName": "Test Printer",
  "manufacturer": "Test Printer Manufacturer",
  "model": "Test Printer Model",
  "physicalDeviceId": null,
  "hasPhysicalDevice": false,
  "certificateSigningRequest": { 
    "content": "{content}",
    "transportKey": "{sampleTransportKey}"
  },
  "connectorId": null
}
```

### <a name="response"></a><span data-ttu-id="7f0a0-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f0a0-173">Response</span></span>
<span data-ttu-id="7f0a0-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7f0a0-174">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Operation-Location: https://graph.microsoft.com/beta/print/operations/f221760a-52e8-4c11-b8c5-5dfaef3a49db
Retry-After: 5
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printers: create",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
