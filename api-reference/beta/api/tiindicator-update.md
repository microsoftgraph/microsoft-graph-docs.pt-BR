---
title: Atualizar tiIndicator
description: Atualizar as propriedades de um objeto tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 3ded1ad2ac77cfd08320c54480de5dd24d319b91
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176952"
---
# <a name="update-tiindicator"></a><span data-ttu-id="45eec-103">Atualizar tiIndicator</span><span class="sxs-lookup"><span data-stu-id="45eec-103">Update tiIndicator</span></span>

<span data-ttu-id="45eec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45eec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45eec-105">Atualizar as propriedades de um [objeto tiIndicator.](../resources/tiindicator.md)</span><span class="sxs-lookup"><span data-stu-id="45eec-105">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="45eec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="45eec-106">Permissions</span></span>

<span data-ttu-id="45eec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45eec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="45eec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45eec-109">Permission type</span></span>                        | <span data-ttu-id="45eec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45eec-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="45eec-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45eec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="45eec-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="45eec-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="45eec-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45eec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45eec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45eec-114">Not supported.</span></span> |
| <span data-ttu-id="45eec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45eec-115">Application</span></span>                            | <span data-ttu-id="45eec-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="45eec-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="45eec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45eec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="45eec-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45eec-118">Request headers</span></span>

| <span data-ttu-id="45eec-119">Nome</span><span class="sxs-lookup"><span data-stu-id="45eec-119">Name</span></span>       | <span data-ttu-id="45eec-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="45eec-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="45eec-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="45eec-121">Authorization</span></span> | <span data-ttu-id="45eec-122">Portador {code} **Obrigatório**</span><span class="sxs-lookup"><span data-stu-id="45eec-122">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="45eec-123">Preferir</span><span class="sxs-lookup"><span data-stu-id="45eec-123">Prefer</span></span> | <span data-ttu-id="45eec-124">return=representation</span><span class="sxs-lookup"><span data-stu-id="45eec-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="45eec-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45eec-125">Request body</span></span>

<span data-ttu-id="45eec-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="45eec-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="45eec-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="45eec-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="45eec-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="45eec-128">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="45eec-129">Os campos obrigatórios são: `id` , `expirationDateTime` . `targetProduct`</span><span class="sxs-lookup"><span data-stu-id="45eec-129">Required fields are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="45eec-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45eec-130">Property</span></span>     | <span data-ttu-id="45eec-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="45eec-131">Type</span></span>        | <span data-ttu-id="45eec-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="45eec-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="45eec-133">ação</span><span class="sxs-lookup"><span data-stu-id="45eec-133">action</span></span>|<span data-ttu-id="45eec-134">string</span><span class="sxs-lookup"><span data-stu-id="45eec-134">string</span></span>| <span data-ttu-id="45eec-135">A ação a ser aplicada se o indicador for corresponder de dentro da ferramenta de segurança targetProduct.</span><span class="sxs-lookup"><span data-stu-id="45eec-135">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="45eec-136">Os valores possíveis são: `unknown`, `allow`, `block`, `alert`.</span><span class="sxs-lookup"><span data-stu-id="45eec-136">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="45eec-137">activityGroupNames</span><span class="sxs-lookup"><span data-stu-id="45eec-137">activityGroupNames</span></span>|<span data-ttu-id="45eec-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="45eec-138">String collection</span></span>|<span data-ttu-id="45eec-139">Os nomes de inteligência contra ameaças cibernéticas para as partes responsáveis pelas atividades mal-intencionadas cobertas pelo indicador de ameaças.</span><span class="sxs-lookup"><span data-stu-id="45eec-139">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="45eec-140">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="45eec-140">additionalInformation</span></span>|<span data-ttu-id="45eec-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45eec-141">String</span></span>|<span data-ttu-id="45eec-142">Uma área catchall na qual dados extras do indicador não cobertos pelas outras propriedades tiIndicator podem ser colocados.</span><span class="sxs-lookup"><span data-stu-id="45eec-142">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="45eec-143">Os dados colocados em additionalInformation normalmente não serão utilizados pela ferramenta de segurança targetProduct.</span><span class="sxs-lookup"><span data-stu-id="45eec-143">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="45eec-144">confidence</span><span class="sxs-lookup"><span data-stu-id="45eec-144">confidence</span></span>|<span data-ttu-id="45eec-145">Int32</span><span class="sxs-lookup"><span data-stu-id="45eec-145">Int32</span></span>|<span data-ttu-id="45eec-146">Um inteiro que representa a confiança dos dados no indicador identifica com precisão o comportamento mal-intencionado.</span><span class="sxs-lookup"><span data-stu-id="45eec-146">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="45eec-147">Os valores aceitáveis são de 0 a 100, sendo 100 o maior.</span><span class="sxs-lookup"><span data-stu-id="45eec-147">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="45eec-148">description</span><span class="sxs-lookup"><span data-stu-id="45eec-148">description</span></span>|<span data-ttu-id="45eec-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45eec-149">String</span></span>|<span data-ttu-id="45eec-150">Breve descrição (100 caracteres ou menos) da ameaça representada pelo indicador.</span><span class="sxs-lookup"><span data-stu-id="45eec-150">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="45eec-151">diamondModel</span><span class="sxs-lookup"><span data-stu-id="45eec-151">diamondModel</span></span>|[<span data-ttu-id="45eec-152">diamondModel</span><span class="sxs-lookup"><span data-stu-id="45eec-152">diamondModel</span></span>](../resources/tiindicator.md#diamondmodel-values)|<span data-ttu-id="45eec-153">A área do Modelo de Losango na qual esse indicador existe.</span><span class="sxs-lookup"><span data-stu-id="45eec-153">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="45eec-154">Os valores possíveis são: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span><span class="sxs-lookup"><span data-stu-id="45eec-154">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="45eec-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="45eec-155">expirationDateTime</span></span>|<span data-ttu-id="45eec-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45eec-156">DateTimeOffset</span></span>| <span data-ttu-id="45eec-157">Cadeia de caracteres DateTime que indica quando o Indicador expira.</span><span class="sxs-lookup"><span data-stu-id="45eec-157">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="45eec-158">Todos os indicadores devem ter uma data de expiração para evitar que os indicadores persistentes persistam no sistema.</span><span class="sxs-lookup"><span data-stu-id="45eec-158">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="45eec-159">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="45eec-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="45eec-160">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="45eec-160">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="45eec-161">externalId</span><span class="sxs-lookup"><span data-stu-id="45eec-161">externalId</span></span>|<span data-ttu-id="45eec-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45eec-162">String</span></span>|<span data-ttu-id="45eec-163">Um número de identificação que vincula o indicador de volta ao sistema do provedor do indicador (por exemplo, uma chave estrangeira).</span><span class="sxs-lookup"><span data-stu-id="45eec-163">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="45eec-164">isActive</span><span class="sxs-lookup"><span data-stu-id="45eec-164">isActive</span></span>|<span data-ttu-id="45eec-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="45eec-165">Boolean</span></span>|<span data-ttu-id="45eec-166">Usado para desativar indicadores no sistema.</span><span class="sxs-lookup"><span data-stu-id="45eec-166">Used to deactivate indicators within system.</span></span> <span data-ttu-id="45eec-167">Por padrão, qualquer indicador enviado é definido como ativo.</span><span class="sxs-lookup"><span data-stu-id="45eec-167">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="45eec-168">No entanto, os provedores podem enviar indicadores existentes com esse conjunto como "Falso" para desativar os indicadores no sistema.</span><span class="sxs-lookup"><span data-stu-id="45eec-168">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="45eec-169">killChain</span><span class="sxs-lookup"><span data-stu-id="45eec-169">killChain</span></span>|<span data-ttu-id="45eec-170">[Coleção killChain](../resources/tiindicator.md#killchain-values)</span><span class="sxs-lookup"><span data-stu-id="45eec-170">[killChain](../resources/tiindicator.md#killchain-values) collection</span></span>|<span data-ttu-id="45eec-171">Uma matriz JSON de cadeias de caracteres que descreve qual ponto ou pontos no Kill Chain esse indicador se direciona.</span><span class="sxs-lookup"><span data-stu-id="45eec-171">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="45eec-172">Consulte "valores killChain" abaixo para saber os valores exatos.</span><span class="sxs-lookup"><span data-stu-id="45eec-172">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="45eec-173">knownFalsePositives</span><span class="sxs-lookup"><span data-stu-id="45eec-173">knownFalsePositives</span></span>|<span data-ttu-id="45eec-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45eec-174">String</span></span>|<span data-ttu-id="45eec-175">Cenários em que o indicador pode causar falsos positivos.</span><span class="sxs-lookup"><span data-stu-id="45eec-175">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="45eec-176">Deve ser um texto acessível para humanos.</span><span class="sxs-lookup"><span data-stu-id="45eec-176">This should be human-readable text.</span></span>|
|<span data-ttu-id="45eec-177">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="45eec-177">lastReportedDateTime</span></span>|<span data-ttu-id="45eec-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45eec-178">DateTimeOffset</span></span>|<span data-ttu-id="45eec-179">A última vez em que o indicador foi visto.</span><span class="sxs-lookup"><span data-stu-id="45eec-179">The last time the indicator was seen.</span></span> <span data-ttu-id="45eec-180">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="45eec-180">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="45eec-181">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="45eec-181">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="45eec-182">malwareFamilyNames</span><span class="sxs-lookup"><span data-stu-id="45eec-182">malwareFamilyNames</span></span>|<span data-ttu-id="45eec-183">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="45eec-183">String collection</span></span>|<span data-ttu-id="45eec-184">O nome da família de malware associado a um indicador, se ele existir.</span><span class="sxs-lookup"><span data-stu-id="45eec-184">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="45eec-185">A Microsoft prefere o nome da família de malware da Microsoft, [](https://www.microsoft.com/wdsi/threats)se possível, que pode ser encontrado por meio da ameaça de inteligência de segurança do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="45eec-185">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="45eec-186">passiveOnly</span><span class="sxs-lookup"><span data-stu-id="45eec-186">passiveOnly</span></span>|<span data-ttu-id="45eec-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="45eec-187">Boolean</span></span>|<span data-ttu-id="45eec-188">Determina se o indicador deve disparar um evento visível para um usuário final.</span><span class="sxs-lookup"><span data-stu-id="45eec-188">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="45eec-189">Quando definido como "verdadeiro", as ferramentas de segurança não notificarão o usuário final de que ocorreu um 'acerto'.</span><span class="sxs-lookup"><span data-stu-id="45eec-189">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="45eec-190">Isso é tratado com mais frequência como modo de auditoria ou silencioso por produtos de segurança, onde eles simplesmente registram que uma combinação ocorreu, mas não executarão a ação.</span><span class="sxs-lookup"><span data-stu-id="45eec-190">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="45eec-191">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="45eec-191">Default value is false.</span></span>|
|<span data-ttu-id="45eec-192">severity</span><span class="sxs-lookup"><span data-stu-id="45eec-192">severity</span></span>|<span data-ttu-id="45eec-193">Int32</span><span class="sxs-lookup"><span data-stu-id="45eec-193">Int32</span></span>|<span data-ttu-id="45eec-194">Um inteiro que representa a gravidade do comportamento mal-intencionado identificado pelos dados dentro do indicador.</span><span class="sxs-lookup"><span data-stu-id="45eec-194">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="45eec-195">Os valores aceitáveis são de 0 a 5, onde 5 é o mais grave e zero não é grave.</span><span class="sxs-lookup"><span data-stu-id="45eec-195">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="45eec-196">O valor padrão é 3.</span><span class="sxs-lookup"><span data-stu-id="45eec-196">Default value is 3.</span></span>|
|<span data-ttu-id="45eec-197">tags</span><span class="sxs-lookup"><span data-stu-id="45eec-197">tags</span></span>|<span data-ttu-id="45eec-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="45eec-198">String collection</span></span>|<span data-ttu-id="45eec-199">Uma matriz JSON de cadeias de caracteres que armazena marcas/palavras-chave arbitrárias.</span><span class="sxs-lookup"><span data-stu-id="45eec-199">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="45eec-200">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="45eec-200">tlpLevel</span></span>|[<span data-ttu-id="45eec-201">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="45eec-201">tlpLevel</span></span>](../resources/tiindicator.md#tlplevel-values)| <span data-ttu-id="45eec-202">Valor do Protocolo semáforo para o indicador.</span><span class="sxs-lookup"><span data-stu-id="45eec-202">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="45eec-203">Os valores possíveis são: `unknown`, `white`, `green`, `amber`, `red`.</span><span class="sxs-lookup"><span data-stu-id="45eec-203">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|


## <a name="response"></a><span data-ttu-id="45eec-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="45eec-204">Response</span></span>

<span data-ttu-id="45eec-205">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="45eec-205">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="45eec-206">Se o header de solicitação opcional for usado, o método retornará um código de resposta e o objeto `200 OK` [tiIndicator](../resources/tiindicator.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45eec-206">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45eec-207">Exemplos</span><span class="sxs-lookup"><span data-stu-id="45eec-207">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="45eec-208">Exemplo 1: Solicitação sem o header Prefer</span><span class="sxs-lookup"><span data-stu-id="45eec-208">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="45eec-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45eec-209">Request</span></span>

<span data-ttu-id="45eec-210">A seguir está um exemplo da solicitação sem `Prefer` o header.</span><span class="sxs-lookup"><span data-stu-id="45eec-210">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="http"></a>[<span data-ttu-id="45eec-211">HTTP</span><span class="sxs-lookup"><span data-stu-id="45eec-211">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json

{
  "description": "description-updated",
}
```
# <a name="c"></a>[<span data-ttu-id="45eec-212">C#</span><span class="sxs-lookup"><span data-stu-id="45eec-212">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45eec-213">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45eec-213">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45eec-214">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45eec-214">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45eec-215">Java</span><span class="sxs-lookup"><span data-stu-id="45eec-215">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="45eec-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="45eec-216">Response</span></span>

<span data-ttu-id="45eec-217">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="45eec-217">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="45eec-218">Exemplo 2: Solicitação com o header Prefer</span><span class="sxs-lookup"><span data-stu-id="45eec-218">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="45eec-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45eec-219">Request</span></span>

<span data-ttu-id="45eec-220">A seguir está um exemplo da solicitação que inclui `Prefer` o header.</span><span class="sxs-lookup"><span data-stu-id="45eec-220">The following is an example of the request that includes the `Prefer` header.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json
Prefer: return=representation

{
  "additionalInformation": "additionalInformation-after-update",
  "confidence": 42,
  "description": "description-after-update",
}
```

#### <a name="response"></a><span data-ttu-id="45eec-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="45eec-221">Response</span></span>

<span data-ttu-id="45eec-222">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="45eec-222">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="45eec-223">O objeto response mostrado aqui pode ser encurtado para maior leitura.</span><span class="sxs-lookup"><span data-stu-id="45eec-223">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="45eec-224">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45eec-224">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXXXXXXX",
    "action": null,
    "additionalInformation": "additionalInformation-after-update",
    "activityGroupNames": [],
    "confidence": 42,
    "description": "description-after-update",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


