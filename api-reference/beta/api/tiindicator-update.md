---
title: Atualizar tiIndicator
description: Atualiza as propriedades de um objeto tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 55613e3c13695a502b43c127c1164d2adf9f6534
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544397"
---
# <a name="update-tiindicator"></a><span data-ttu-id="ddf69-103">Atualizar tiIndicator</span><span class="sxs-lookup"><span data-stu-id="ddf69-103">Update tiIndicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddf69-104">Atualiza as propriedades de um objeto [tiIndicator](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="ddf69-104">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddf69-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ddf69-105">Permissions</span></span>

<span data-ttu-id="ddf69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddf69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ddf69-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddf69-108">Permission type</span></span>                        | <span data-ttu-id="ddf69-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddf69-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ddf69-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddf69-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ddf69-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="ddf69-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="ddf69-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddf69-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddf69-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddf69-113">Not supported.</span></span> |
| <span data-ttu-id="ddf69-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddf69-114">Application</span></span>                            | <span data-ttu-id="ddf69-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="ddf69-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddf69-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddf69-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ddf69-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf69-117">Request headers</span></span>

| <span data-ttu-id="ddf69-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ddf69-118">Name</span></span>       | <span data-ttu-id="ddf69-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddf69-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ddf69-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddf69-120">Authorization</span></span> | <span data-ttu-id="ddf69-121">Portador {código} **obrigatório**</span><span class="sxs-lookup"><span data-stu-id="ddf69-121">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="ddf69-122">Preferir</span><span class="sxs-lookup"><span data-stu-id="ddf69-122">Prefer</span></span> | <span data-ttu-id="ddf69-123">Return = representação</span><span class="sxs-lookup"><span data-stu-id="ddf69-123">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddf69-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf69-124">Request body</span></span>

<span data-ttu-id="ddf69-125">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="ddf69-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ddf69-126">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="ddf69-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ddf69-127">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ddf69-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ddf69-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddf69-128">Property</span></span>     | <span data-ttu-id="ddf69-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddf69-129">Type</span></span>        | <span data-ttu-id="ddf69-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddf69-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ddf69-131">ação</span><span class="sxs-lookup"><span data-stu-id="ddf69-131">action</span></span>|<span data-ttu-id="ddf69-132">string</span><span class="sxs-lookup"><span data-stu-id="ddf69-132">string</span></span>| <span data-ttu-id="ddf69-133">A ação a ser aplicada se o indicador for correspondido de dentro da ferramenta de segurança do targetProduct.</span><span class="sxs-lookup"><span data-stu-id="ddf69-133">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="ddf69-134">Os valores possíveis são: `unknown`, `allow`, `block`, `alert`.</span><span class="sxs-lookup"><span data-stu-id="ddf69-134">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="ddf69-135">activityGroupNames</span><span class="sxs-lookup"><span data-stu-id="ddf69-135">activityGroupNames</span></span>|<span data-ttu-id="ddf69-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddf69-136">String collection</span></span>|<span data-ttu-id="ddf69-137">O nome do Cyber Threat Intelligence (s) para as partes responsáveis pela atividade mal-intencionada coberta pelo indicador de ameaças.</span><span class="sxs-lookup"><span data-stu-id="ddf69-137">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="ddf69-138">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="ddf69-138">additionalInformation</span></span>|<span data-ttu-id="ddf69-139">String</span><span class="sxs-lookup"><span data-stu-id="ddf69-139">String</span></span>|<span data-ttu-id="ddf69-140">Uma área catchall na qual os dados extras do indicador não cobertos pelas outras propriedades de tiIndicator podem ser colocados.</span><span class="sxs-lookup"><span data-stu-id="ddf69-140">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="ddf69-141">Os dados colocados no additionalInformation normalmente não serão utilizados pela ferramenta de segurança do targetProduct.</span><span class="sxs-lookup"><span data-stu-id="ddf69-141">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="ddf69-142">confidence</span><span class="sxs-lookup"><span data-stu-id="ddf69-142">confidence</span></span>|<span data-ttu-id="ddf69-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ddf69-143">Int32</span></span>|<span data-ttu-id="ddf69-144">Um inteiro representando a confiança dos dados dentro do indicador identifica precisamente o comportamento mal-intencionado.</span><span class="sxs-lookup"><span data-stu-id="ddf69-144">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="ddf69-145">Os valores aceitáveis são 0 – 100 com 100 sendo os mais altos.</span><span class="sxs-lookup"><span data-stu-id="ddf69-145">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="ddf69-146">description</span><span class="sxs-lookup"><span data-stu-id="ddf69-146">description</span></span>|<span data-ttu-id="ddf69-147">String</span><span class="sxs-lookup"><span data-stu-id="ddf69-147">String</span></span>|<span data-ttu-id="ddf69-148">Breve descrição (100 caracteres ou menos) da ameaça representada pelo indicador.</span><span class="sxs-lookup"><span data-stu-id="ddf69-148">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="ddf69-149">diamondModel</span><span class="sxs-lookup"><span data-stu-id="ddf69-149">diamondModel</span></span>|[<span data-ttu-id="ddf69-150">diamondModel</span><span class="sxs-lookup"><span data-stu-id="ddf69-150">diamondModel</span></span>](#diamondmodel-values)|<span data-ttu-id="ddf69-151">A área do modelo em losango em que esse indicador existe.</span><span class="sxs-lookup"><span data-stu-id="ddf69-151">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="ddf69-152">Os valores possíveis são: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span><span class="sxs-lookup"><span data-stu-id="ddf69-152">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="ddf69-153">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ddf69-153">expirationDateTime</span></span>|<span data-ttu-id="ddf69-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddf69-154">DateTimeOffset</span></span>| <span data-ttu-id="ddf69-155">Cadeia de caracteres DateTime indicando quando o indicador expira.</span><span class="sxs-lookup"><span data-stu-id="ddf69-155">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="ddf69-156">Todos os indicadores devem ter uma data de vencimento para evitar indicadores obsoletos persistentes no sistema.</span><span class="sxs-lookup"><span data-stu-id="ddf69-156">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="ddf69-157">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ddf69-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ddf69-158">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="ddf69-158">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="ddf69-159">externalId</span><span class="sxs-lookup"><span data-stu-id="ddf69-159">externalId</span></span>|<span data-ttu-id="ddf69-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddf69-160">String</span></span>|<span data-ttu-id="ddf69-161">Um número de identificação que liga o indicador de volta para o sistema do provedor de indicadores (por exemplo, uma chave externa).</span><span class="sxs-lookup"><span data-stu-id="ddf69-161">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="ddf69-162">isActive</span><span class="sxs-lookup"><span data-stu-id="ddf69-162">isActive</span></span>|<span data-ttu-id="ddf69-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="ddf69-163">Boolean</span></span>|<span data-ttu-id="ddf69-164">Usado para desativar indicadores no sistema.</span><span class="sxs-lookup"><span data-stu-id="ddf69-164">Used to deactivate indicators within system.</span></span> <span data-ttu-id="ddf69-165">Por padrão, qualquer indicador enviado é definido como ativo.</span><span class="sxs-lookup"><span data-stu-id="ddf69-165">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="ddf69-166">No enTanto, os provedores podem enviar indicadores existentes com este conjunto como ' false ' para desativar indicadores no sistema.</span><span class="sxs-lookup"><span data-stu-id="ddf69-166">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="ddf69-167">killChain</span><span class="sxs-lookup"><span data-stu-id="ddf69-167">killChain</span></span>|<span data-ttu-id="ddf69-168">coleção [killChain](#killchain-values)</span><span class="sxs-lookup"><span data-stu-id="ddf69-168">[killChain](#killchain-values) collection</span></span>|<span data-ttu-id="ddf69-169">Uma matriz JSON de cadeias de caracteres que descreve o ponto ou os pontos na cadeia de Kill que este indicador aponta.</span><span class="sxs-lookup"><span data-stu-id="ddf69-169">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="ddf69-170">Consulte "valores de killChain" abaixo para ver os valores exatos.</span><span class="sxs-lookup"><span data-stu-id="ddf69-170">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="ddf69-171">knownFalsePositives</span><span class="sxs-lookup"><span data-stu-id="ddf69-171">knownFalsePositives</span></span>|<span data-ttu-id="ddf69-172">String</span><span class="sxs-lookup"><span data-stu-id="ddf69-172">String</span></span>|<span data-ttu-id="ddf69-173">Cenários nos quais o indicador pode causar falsos positivos.</span><span class="sxs-lookup"><span data-stu-id="ddf69-173">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="ddf69-174">Isso deve ser um texto legível por pessoas.</span><span class="sxs-lookup"><span data-stu-id="ddf69-174">This should be human-readable text.</span></span>|
|<span data-ttu-id="ddf69-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddf69-175">lastReportedDateTime</span></span>|<span data-ttu-id="ddf69-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddf69-176">DateTimeOffset</span></span>|<span data-ttu-id="ddf69-177">A última vez que o indicador foi visto.</span><span class="sxs-lookup"><span data-stu-id="ddf69-177">The last time the indicator was seen.</span></span> <span data-ttu-id="ddf69-178">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ddf69-178">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ddf69-179">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="ddf69-179">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="ddf69-180">malwareFamilyNames</span><span class="sxs-lookup"><span data-stu-id="ddf69-180">malwareFamilyNames</span></span>|<span data-ttu-id="ddf69-181">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddf69-181">String collection</span></span>|<span data-ttu-id="ddf69-182">O nome da família de malware associado a um indicador, se existir.</span><span class="sxs-lookup"><span data-stu-id="ddf69-182">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="ddf69-183">A Microsoft prefere o nome da família de malware da Microsoft, se possível, que possa ser encontrado por meio da [enciclopédia de ameaças](https://www.microsoft.com/wdsi/threats)de inteligência de segurança do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="ddf69-183">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="ddf69-184">passiveOnly</span><span class="sxs-lookup"><span data-stu-id="ddf69-184">passiveOnly</span></span>|<span data-ttu-id="ddf69-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="ddf69-185">Boolean</span></span>|<span data-ttu-id="ddf69-186">Determina se o indicador deve acionar um evento que é visível para um usuário final.</span><span class="sxs-lookup"><span data-stu-id="ddf69-186">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="ddf69-187">Quando definido como ' true ', as ferramentas de segurança não notificarão o usuário final de que um ' hit ' ocorreu.</span><span class="sxs-lookup"><span data-stu-id="ddf69-187">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="ddf69-188">Isso geralmente é tratado como um modo de auditoria ou silencioso por produtos de segurança onde eles simplesmente farão o registro de que uma correspondência ocorreu, mas não executará a ação.</span><span class="sxs-lookup"><span data-stu-id="ddf69-188">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="ddf69-189">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="ddf69-189">Default value is false.</span></span>|
|<span data-ttu-id="ddf69-190">severity</span><span class="sxs-lookup"><span data-stu-id="ddf69-190">severity</span></span>|<span data-ttu-id="ddf69-191">Int32</span><span class="sxs-lookup"><span data-stu-id="ddf69-191">Int32</span></span>|<span data-ttu-id="ddf69-192">Um inteiro que representa a gravidade do comportamento mal-intencionado identificado pelos dados dentro do indicador.</span><span class="sxs-lookup"><span data-stu-id="ddf69-192">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="ddf69-193">Os valores aceitáveis são 0 – 5, onde 5 é o mais grave e zero não é grave.</span><span class="sxs-lookup"><span data-stu-id="ddf69-193">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="ddf69-194">O valor padrão é 3.</span><span class="sxs-lookup"><span data-stu-id="ddf69-194">Default value is 3.</span></span>|
|<span data-ttu-id="ddf69-195">tags</span><span class="sxs-lookup"><span data-stu-id="ddf69-195">tags</span></span>|<span data-ttu-id="ddf69-196">String collection</span><span class="sxs-lookup"><span data-stu-id="ddf69-196">String collection</span></span>|<span data-ttu-id="ddf69-197">Uma matriz JSON de cadeias de caracteres que armazena marcas arbitrárias/palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="ddf69-197">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="ddf69-198">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="ddf69-198">tlpLevel</span></span>|[<span data-ttu-id="ddf69-199">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="ddf69-199">tlpLevel</span></span>](#tlplevel-values)| <span data-ttu-id="ddf69-200">Valor do protocolo de luz de tráfego para o indicador.</span><span class="sxs-lookup"><span data-stu-id="ddf69-200">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="ddf69-201">Os valores possíveis são: `unknown`, `white`, `green`, `amber`, `red`.</span><span class="sxs-lookup"><span data-stu-id="ddf69-201">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|

### <a name="diamondmodel-values"></a><span data-ttu-id="ddf69-202">valores de diamondModel</span><span class="sxs-lookup"><span data-stu-id="ddf69-202">diamondModel values</span></span>

<span data-ttu-id="ddf69-203">Para obter informações sobre esse modelo, consulte [o modelo de losango](http://diamondmodel.org).</span><span class="sxs-lookup"><span data-stu-id="ddf69-203">For information about this model, see [The diamond model](http://diamondmodel.org).</span></span>

| <span data-ttu-id="ddf69-204">Valores</span><span class="sxs-lookup"><span data-stu-id="ddf69-204">Values</span></span> | <span data-ttu-id="ddf69-205">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddf69-205">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="ddf69-206">adversário</span><span class="sxs-lookup"><span data-stu-id="ddf69-206">adversary</span></span>|<span data-ttu-id="ddf69-207">O indicador descreve o adversário.</span><span class="sxs-lookup"><span data-stu-id="ddf69-207">The indicator describes the adversary.</span></span>|
|<span data-ttu-id="ddf69-208">função</span><span class="sxs-lookup"><span data-stu-id="ddf69-208">capability</span></span>|<span data-ttu-id="ddf69-209">O indicador é uma capacidade do adversário.</span><span class="sxs-lookup"><span data-stu-id="ddf69-209">The indicator is a capability of the adversary.</span></span>|
|<span data-ttu-id="ddf69-210">ti</span><span class="sxs-lookup"><span data-stu-id="ddf69-210">infrastructure</span></span>|<span data-ttu-id="ddf69-211">O indicador descreve a infraestrutura do adversário.</span><span class="sxs-lookup"><span data-stu-id="ddf69-211">The indicator describes infrastructure of the adversary.</span></span>|
|<span data-ttu-id="ddf69-212">vítima</span><span class="sxs-lookup"><span data-stu-id="ddf69-212">victim</span></span>|<span data-ttu-id="ddf69-213">O indicador descreve a vítima do adversário.</span><span class="sxs-lookup"><span data-stu-id="ddf69-213">The indicator describes the victim of the adversary.</span></span>|

### <a name="killchain-values"></a><span data-ttu-id="ddf69-214">valores de killChain</span><span class="sxs-lookup"><span data-stu-id="ddf69-214">killChain values</span></span>

| <span data-ttu-id="ddf69-215">Valores</span><span class="sxs-lookup"><span data-stu-id="ddf69-215">Values</span></span> | <span data-ttu-id="ddf69-216">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddf69-216">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="ddf69-217">Actions</span><span class="sxs-lookup"><span data-stu-id="ddf69-217">Actions</span></span>|<span data-ttu-id="ddf69-218">Representa "ações nos objetivos".</span><span class="sxs-lookup"><span data-stu-id="ddf69-218">Represents “Actions on Objectives”.</span></span> <span data-ttu-id="ddf69-219">O invasor está aproveitando o sistema comprometido para realizar ações como um ataque de negação de serviço distribuído.</span><span class="sxs-lookup"><span data-stu-id="ddf69-219">The attacker is leveraging the compromised system to take actions such as a distributed denial of service attack.</span></span>|
|<span data-ttu-id="ddf69-220">C2</span><span class="sxs-lookup"><span data-stu-id="ddf69-220">C2</span></span>|<span data-ttu-id="ddf69-221">Representa o canal de controle pelo qual um sistema comprometido é manipulado.</span><span class="sxs-lookup"><span data-stu-id="ddf69-221">Represents the control channel by which a compromised system is manipulated.</span></span>|
|<span data-ttu-id="ddf69-222">Entrega</span><span class="sxs-lookup"><span data-stu-id="ddf69-222">Delivery</span></span>|<span data-ttu-id="ddf69-223">O processo de distribuição do código de exploração para vítimas (por exemplo, USB, email, sites).</span><span class="sxs-lookup"><span data-stu-id="ddf69-223">The process of distributing the exploit code to victims (for example USB, email, websites).</span></span>|
|<span data-ttu-id="ddf69-224">Invasão</span><span class="sxs-lookup"><span data-stu-id="ddf69-224">Exploitation</span></span>|<span data-ttu-id="ddf69-225">O código de exploração que aproveita as vulnerabilidades (por exemplo, execução de código).</span><span class="sxs-lookup"><span data-stu-id="ddf69-225">The exploit code taking advantage of vulnerabilities (for example, code execution).</span></span>|
|<span data-ttu-id="ddf69-226">Instalação</span><span class="sxs-lookup"><span data-stu-id="ddf69-226">Installation</span></span>|<span data-ttu-id="ddf69-227">Instalação de malware após uma vulnerabilidade ter sido explorada.</span><span class="sxs-lookup"><span data-stu-id="ddf69-227">Installing malware after a vulnerability has been exploited.</span></span>|
|<span data-ttu-id="ddf69-228">Reconhecimento</span><span class="sxs-lookup"><span data-stu-id="ddf69-228">Reconnaissance</span></span>|<span data-ttu-id="ddf69-229">O indicador é uma evidência de um grupo de atividades que coleta informações a serem usadas em um ataque futuro.</span><span class="sxs-lookup"><span data-stu-id="ddf69-229">Indicator is evidence of an activity group harvesting information to be used in a future attack.</span></span>|
|<span data-ttu-id="ddf69-230">Armas</span><span class="sxs-lookup"><span data-stu-id="ddf69-230">Weaponization</span></span>|<span data-ttu-id="ddf69-231">Transformar uma vulnerabilidade em código de exploração (por exemplo, malware).</span><span class="sxs-lookup"><span data-stu-id="ddf69-231">Turning a vulnerability into exploit code (for example, malware).</span></span>|

### <a name="tlplevel-values"></a><span data-ttu-id="ddf69-232">valores de tlpLevel</span><span class="sxs-lookup"><span data-stu-id="ddf69-232">tlpLevel values</span></span>

<span data-ttu-id="ddf69-233">Todos os indicadores devem ter um valor de protocolo de semáforo (TLP) quando ele é enviado.</span><span class="sxs-lookup"><span data-stu-id="ddf69-233">Every indicator must have a Traffic Light Protocol (tlp) value when it is submitted.</span></span> <span data-ttu-id="ddf69-234">Esse valor representa a sensibilidade e o escopo de compartilhamento de um determinado indicador.</span><span class="sxs-lookup"><span data-stu-id="ddf69-234">This value represents the sensitivity and sharing scope of a given indicator.</span></span>

| <span data-ttu-id="ddf69-235">Valores</span><span class="sxs-lookup"><span data-stu-id="ddf69-235">Values</span></span> | <span data-ttu-id="ddf69-236">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddf69-236">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="ddf69-237">Branco</span><span class="sxs-lookup"><span data-stu-id="ddf69-237">White</span></span>| <span data-ttu-id="ddf69-238">Escopo de compartilhamento: ilimitado.</span><span class="sxs-lookup"><span data-stu-id="ddf69-238">Sharing scope: Unlimited.</span></span> <span data-ttu-id="ddf69-239">Os indicadores podem ser compartilhados livremente, sem restrição.</span><span class="sxs-lookup"><span data-stu-id="ddf69-239">Indicators can be shared freely, without restriction.</span></span>|
|<span data-ttu-id="ddf69-240">Verde</span><span class="sxs-lookup"><span data-stu-id="ddf69-240">Green</span></span>| <span data-ttu-id="ddf69-241">Escopo de compartilhamento: Comunidade.</span><span class="sxs-lookup"><span data-stu-id="ddf69-241">Sharing scope: Community.</span></span> <span data-ttu-id="ddf69-242">Os indicadores podem ser compartilhados com a comunidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="ddf69-242">Indicators can be shared with the security community.</span></span>|
|<span data-ttu-id="ddf69-243">Âmbar</span><span class="sxs-lookup"><span data-stu-id="ddf69-243">Amber</span></span>| <span data-ttu-id="ddf69-244">Escopo de compartilhamento: limitado.</span><span class="sxs-lookup"><span data-stu-id="ddf69-244">Sharing scope: Limited.</span></span> <span data-ttu-id="ddf69-245">Essa é a configuração padrão para indicadores e restringe o compartilhamento apenas àqueles que têm de ser conhecidos: 1) serviços e operadores de serviço que implementam inteligência de ameaças; 2) clientes cujos sistemas apresentam comportamento consistente com o indicador.</span><span class="sxs-lookup"><span data-stu-id="ddf69-245">This is the default setting for indicators and restricts sharing to only those with a need-to-know: 1) Services and service operators that implement threat intelligence; 2) Customers whose system(s) exhibit behavior consistent with the indicator.</span></span>|
|<span data-ttu-id="ddf69-246">Vermelho</span><span class="sxs-lookup"><span data-stu-id="ddf69-246">Red</span></span>| <span data-ttu-id="ddf69-247">Escopo de compartilhamento: pessoal.</span><span class="sxs-lookup"><span data-stu-id="ddf69-247">Sharing scope: Personal.</span></span> <span data-ttu-id="ddf69-248">Esses indicadores devem ser compartilhados apenas diretamente e, preferencialmente, em pessoa.</span><span class="sxs-lookup"><span data-stu-id="ddf69-248">These indicators are to only be shared directly and, preferably, in person.</span></span> <span data-ttu-id="ddf69-249">Normalmente, os indicadores vermelhos do TLP não são incluídos devido às restrições predefinidas.</span><span class="sxs-lookup"><span data-stu-id="ddf69-249">Typically, TLP Red indicators are not ingested due to their pre-defined restrictions.</span></span> <span data-ttu-id="ddf69-250">Se TLP indicadores vermelhos forem enviados, a propriedade **passiveOnly** também deverá ser definida `True` como.</span><span class="sxs-lookup"><span data-stu-id="ddf69-250">If TLP Red indicators are submitted, the **passiveOnly** property should be set to `True` as well.</span></span> |

## <a name="response"></a><span data-ttu-id="ddf69-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddf69-251">Response</span></span>

<span data-ttu-id="ddf69-252">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ddf69-252">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="ddf69-253">Se o cabeçalho de solicitação opcional for usado, o método retornará `200 OK` um código de resposta e o objeto [tiIndicator](../resources/tiIndicator.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddf69-253">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiIndicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ddf69-254">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ddf69-254">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="ddf69-255">Exemplo 1: solicitação sem cabeçalho de preferência</span><span class="sxs-lookup"><span data-stu-id="ddf69-255">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="ddf69-256">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf69-256">Request</span></span>

<span data-ttu-id="ddf69-257">Veja a seguir um exemplo da solicitação sem `Prefer` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="ddf69-257">The following is an example of the request without the `Prefer` header.</span></span>
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

#### <a name="response"></a><span data-ttu-id="ddf69-258">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddf69-258">Response</span></span>

<span data-ttu-id="ddf69-259">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddf69-259">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="ddf69-260">Exemplo 2: solicitação com cabeçalho preferencial</span><span class="sxs-lookup"><span data-stu-id="ddf69-260">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="ddf69-261">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf69-261">Request</span></span>

<span data-ttu-id="ddf69-262">Veja a seguir um exemplo da solicitação que inclui o `Prefer` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="ddf69-262">The following is an example of the request that includes the `Prefer` header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="ddf69-263">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddf69-263">Response</span></span>

<span data-ttu-id="ddf69-264">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddf69-264">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="ddf69-265">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ddf69-265">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ddf69-266">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddf69-266">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
