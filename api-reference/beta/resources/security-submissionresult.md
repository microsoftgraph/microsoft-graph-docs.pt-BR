---
title: Tipo de recurso submissionResult
description: Representa o resultado de uma revisão depois que o envio de ameaças é processado pela Microsoft.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 302a37636fa66fae386e660c34d59f72f1ca2e0f
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856571"
---
# <a name="submissionresult-resource-type"></a>Tipo de recurso submissionResult

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o resultado de uma revisão depois que o envio de ameaças é processado pela Microsoft.

## <a name="properties"></a>Propriedades
| Propriedade           | Tipo                               | Descrição                                                             |
|:-------------------|:-----------------------------------|:------------------------------------------------------------------------|
| Ferramentas para desenvolvedores           | submissionResultCategory           | A categoria de resultado do envio. Os valores possíveis são: , , , , , `allowedByPolicy`, `blockedByPolicy`, `spoof`, `unknown`e `unkownFutureValue``noResultAvailable` . `malware``phishing``spam``notJunk` |
| Detalhe             | [security.submissionResultDetail](#submissionresultdetail-values)             | Especifica os detalhes adicionais fornecidos pela Microsoft para confirmar o resultado da análise. |
| detectedFiles      | Collection([security.submissionDetectedFile](../resources/security-submissiondetectedfile.md)) | Especifica os arquivos detectados pela Microsoft nos emails enviados.|
| detectedUrls       | Collection(String)                 | Especifica as URLs detectadas pela Microsoft no email enviado.|
| userMailboxSetting | [security.userMailboxSetting](#usermailboxsetting-values) | Especifica a configuração da caixa de correio do usuário indicada por uma cadeia de caracteres separada por vírgulas. |

### <a name="usermailboxsetting-values"></a>Valores userMailboxSetting
| Member  | Descrição |
| :----------------- | :------------------------------------ |
| none | nenhuma configuração de caixa de correio do usuário relacionada a esse envio de ameaça. |
| junkMailDeletion | o email enviado foi aplicado com a exclusão de lixo eletrônico. |
| isFromAddressInAddressBook | o email enviado era do endereço no catálogo de endereços. |
| isFromAddressInAddressSafeList | o email enviado era do endereço na lista de endereços seguros. |
| isFromAddressInAddressBlockList | o email enviado era do endereço na lista de endereços seguros. |
| isFromAddressInAddressImplicitSafeList | o email enviado era do endereço na lista de segurança implícita do endereço. |
| isFromAddressInAddressImplicitJunkList | o email enviado era do endereço na lista de lixo eletrônico implícito do endereço. |
| isFromDomainInDomainSafeList | o email enviado era do domínio na lista de segurança de domínio. |
| isFromDomainInDomainBlockList | o email enviado era do domínio na lista de bloqueios de domínio. |
| isRecipientInRecipientSafeList | o email enviado era para o destinatário na lista de segurança do destinatário. |
| customRule | o email enviado foi tratado por uma regra personalizada do usuário. |
| senderPraPresent | o email enviado era do remetente que apresenta antes. |
| fromFirstTimeSender | o email enviado foi da primeira vez que o remetente. |
| Exclusivo | o destinatário do email enviado é exclusivo do catálogo de endereços do destinatário, enquanto a entrega só era permitida de contatos do catálogo de endereços. |
| priorSeenPass | o email enviado foi visto anteriormente aprovado. |
| senderAuthenticationSucceeded | a autenticação do remetente do email enviado foi bem-sucedida. |
| isJunkMailRuleEnabled | a regra de lixo eletrônico foi habilitada. |
| unknownFutureValue | valor futuro desconhecido. |

### <a name="submissionresultdetail-values"></a>Valores submissionResultDetail
| Member                                  | Descrição                                                  |
| :------------------------------------- | :----------------------------------------------------------- |
| none                                   | A Microsoft não tem detalhes adicionais sobre o resultado a ser compartilhamento.            |
| underInvestigation                     | A Microsoft ainda está analisando o exemplo e os resultados devem estar disponíveis em breve.      |
| simulatedThreat                        |  A mensagem relatada foi bloqueada, pois é um email simulado de phishing enviado aos usuários para educação de phishing. Para configurar o EOP/MDO para permitir que ele confira a entrega avançada|
| allowedBySecOps                          | A mensagem relatada foi permitida devido ao fluxo de entrega avançado para a caixa de correio de operadores de segurança. Portanto, remova-o da entrega avançada para bloqueiá-lo |
| allowedByThirdPartyFilters             | A mensagem relatada foi permitida/bloqueada devido a filtros de terceiros que funcionam em conjunto com o EOP/MDO. Configurar a filtragem aprimorada para que o EOP/MDO possa filtrar com precisão   |
| messageNotFound                        | A Microsoft não pode fornecer um veredicto sobre a mensagem relatada, pois a Microsoft não pode encontrar a mensagem real. Envie novamente carregando o email usando envios no security.microsoft.com |
| urlFileShouldNotBeBlocked              | A Microsoft localiza a entidade relatada como limpa. Os emails existentes que o contêm foram liberados. Os filtros de phishing e malware aprenderão com isso após algumas semanas. Até lá, para permitir, crie uma entrada de permissão na lista de permissões/bloqueios do locatário, se ainda não tiver feito isso. |
| urlFileShouldBeBlocked                 | A Microsoft considera a entidade relatada mal-intencionada. Os emails existentes que o contêm foram colocados em quarentena. Os filtros de phishing e malware aprenderão com isso após algumas semanas. Até lá, para bloqueiá-lo, crie uma entrada de bloco na lista de permissões/blocos do locatário, se ainda não tiver sido feito |
| urlFileCannotMakeDecision              | A Microsoft não pode chegar a um veredicto no momento. Reenvie-o para obter um veredicto após a análise. Use a lista de permissões/bloqueios de locatário para permitir/bloquear imediatamente, se ainda não tiver feito isso. |
| domainImpersonation                    | A mensagem relatada foi permitida/bloqueada devido às configurações de política de representação de domínio. Configurar a política de representação de domínio para que o EOP/MDO possa filtrar adequadamente |
| userImpersonation                      | A mensagem relatada foi permitida/bloqueada devido às configurações de política de representação do usuário. Configurar a política de representação do usuário para que o EOP/MDO possa filtrar adequadamente |
| brandImpersonation                     | A mensagem relatada foi permitida/bloqueada devido às configurações de política de representação de marca. Configurar a política de representação de marca para que o EOP/MDO possa filtrar adequadamente |
| outboundShouldNotBeBlocked             | As mensagens de saída relatadas foram encontradas limpas e a Microsoft atualizará seus filtros de saída baseados em aprendizado de máquina nas próximas semanas. |
| outboundShouldBeBlocked                | As mensagens de saída relatadas foram encontradas mal-intencionadas e a Microsoft atualizará seus filtros de saída baseados em aprendizado de máquina nas próximas semanas. |
| outboundBulk                           | A Microsoft acha que a mensagem relatada é spam/lixo eletrônico. Os filtros de saída aprenderão após algumas semanas |
| outboundCannotMakeDecision             | A Microsoft não pode chegar a um veredicto no momento. Reenvie-o para chegar a um veredicto após a análise.  |
| outboundNotRescanned                   | A Microsoft não pode fornecer um veredicto sobre a mensagem de saída relatada, pois a Microsoft não pode encontrar a mensagem real. Envie novamente carregando o email usando envios no security.microsoft.com |
| zeroHourAutoPurgeAllowed               | A mensagem relatada foi removida porque a organização tem limpeza automática de zero hora ativada. |
| zeroHourAutoPurgeBlocked               | Não foi possível desativar a mensagem relatada, pois a organização desativou a limpeza automática de zero hora. Ativar a limpeza automática de hora zero para EOP/MDO para zapar mensagens se elas se tornarem mal-intencionadas após a entrega|
| zeroHourAutoPurgeQuarantineReleased    | A mensagem relatada foi liberada da Quarentena, apesar de estar em quarentena devido ao zap à medida que a mensagem se tornou mal-intencionada após a entrega. |
| onPremisesSkip                         | A mensagem relatada não pode ser analisada, pois ela passou por uma configuração inicial da proteção do Exchange Online. Configure sua configuração híbrida para que o EOP/MDO possa verificar mensagens antes de entregar para trocar caixas de correio no local |
| allowedByTenantAllowBlockList          | A mensagem relatada foi permitida, pois uma ou mais entidades no email estão na lista de permissões/bloqueios do locatário. Remover permissões da lista de permissões/bloqueios do locatário para que o EOP/MDO possa filtrar adequadamente |
| blockedByTenantAllowBlockList          | A mensagem relatada foi bloqueada porque uma ou mais entidades no email estão na lista de permissões/bloqueios do locatário. Remover blocos da lista de permissões/bloqueios do locatário para que o EOP/MDO possa filtrar adequadamente |
| allowedUrlByTenantAllowBlockList       | A URL relatada foi permitida como está na lista de permissões/bloqueios do locatário. Remover a permissão da lista de permissões/bloqueios do locatário para que o EOP/MDO possa filtrar adequadamente |
| allowedFileByTenantAllowBlockList      | O arquivo relatado foi permitido como está na lista de permissões/bloqueios do locatário. Remover a permissão da lista de permissões/bloqueios do locatário para que o EOP/MDO possa filtrar adequadamente |
| allowedSenderByTenantAllowBlockList    | A mensagem relatada foi permitida, pois o remetente do email está na lista de permissões/bloqueios do locatário. Remover a permissão da lista de permissões/bloqueios do locatário para que o EOP/MDO possa filtrar adequadamente|
| allowedRecipientByTenantAllowBlockList | A mensagem de saída relatada foi permitida, pois o destinatário está na lista de permissões/bloqueios do locatário. Remover a permissão do locatário de permitir/bloquear para que o EOP/MDO possa filtrar adequadamente |
| blockedUrlByTenantAllowBlockList       | A URL relatada foi bloqueada como está na lista de permissões/bloqueios do locatário. Remover o bloco da lista de permissões/bloqueios do locatário para que o EOP/MDO possa filtrar adequadamente |
| blockedFileByTenantAllowBlockList      | O arquivo relatado foi bloqueado, pois está na lista de permissões/bloqueios do locatário. Remover o bloco da lista de permissões/bloqueios do locatário para que o EOP/MDO possa filtrar adequadamente |
| blockedSenderByTenantAllowBlockList    | A mensagem relatada foi bloqueada porque o remetente do email está na lista de permissões/bloqueios do locatário. Remover bloco da lista de permissões/bloqueios do locatário para que o EOP/MDO possa filtrar adequadamente|
| blockedRecipientByTenantAllowBlockList | A mensagem de saída relatada foi bloqueada, pois o destinatário está na lista de permissões/bloqueios do locatário. Remover o bloco de permissão/bloqueio do locatário para que o EOP/MDO possa filtrar adequadamente |
| allowedByConnection                    | A mensagem relatada foi permitida, pois o IP de envio está na política de filtro de conexão hospedada. Remover o IP da política de filtro de conexão hospedada para que o EOP/MDO possa filtrar adequadamente |
| blockedByConnection                    | A mensagem relatada foi bloqueada porque o IP de envio está na política de filtro de conexão hospedada. Remover o IP da política de filtro de conexão hospedada para que o EOP/MDO possa filtrar adequadamente |
| allowedByExchangeTransportRule         | A mensagem relatada foi permitida, pois a organização tem uma regra de transporte de troca relacionada. Remova a regra de transporte de troca para que o EOP/MDO possa filtrar adequadamente. |
| blockedByExchangeTransportRule         | A mensagem relatada foi bloqueada, pois a organização tem uma regra de transporte de troca relacionada. Remova a regra de transporte de troca para que o EOP/MDO possa filtrar adequadamente. |
| quarantineReleased                     | A mensagem relatada foi liberada da quarentena, apesar de estar em quarentena pelo EOP/MDO |
| quarantineReleasedThenBlocked          | A mensagem relatada foi bloqueada pela configuração do usuário depois de ser liberada da Quarentena. Remover a configuração do usuário para que o email possa ser liberado para a caixa de entrada |
| junkMailRuleDisabled                   | A mensagem relatada estava associada a ser entregue à pasta lixo eletrônico, mas a pasta de lixo eletrônico foi desabilitada. Ativar a configuração de pasta de lixo eletrônico para que o EOP/MDO possa entregar emails adequadamente |
| allowedByUserSetting                   | A mensagem relatada foi permitida devido à configuração de remetente confiável ou seguro do usuário no Outlook. Remover a configuração de remetente confiável ou seguro para que o EOP/MDO possa filtrar adequadamente |
| blockedByUserSetting                   | A mensagem relatada foi bloqueada devido à configuração de remetente confiável ou bloqueado pelo usuário no Outlook. Remover a configuração de remetente bloqueado ou confiável para que o EOP/MDO possa filtrar adequadamente |
| allowedByTenant                        | A mensagem relatada foi permitida devido a configurações de política de locatário ou de ação de política. Examine as configurações de política ou ação de política EOP/MDO para que o EOP/MDO possa filtrar adequadamente |
| blockedByTenant                        | A mensagem relatada foi bloqueada devido à política de locatário ou às configurações de ação da política. Examine as configurações de política ou ação de política EOP/MDO para que o EOP/MDO possa filtrar adequadamente |
| invalidFalsePositive                   | A mensagem relatada já é permitida pelo EOP/MDO.                  |
| invalidFalseNegative                   | A mensagem relatada já está bloqueada pelo EOP/MDO.                     |
| spoofBlocked                           | A mensagem relatada foi determinada por falsificação pelo nosso sistema e, portanto, bloqueada. Criar uma permissão de falsificação na lista de permissões/bloqueios de locatário para que o EOP/MDO possa permitir emails desse remetente falsificado    |
| goodReclassifiedAsBad                  | A Microsoft considera a mensagem relatada mal-intencionada. Emails existentes foram colocados em quarentena. Os filtros de phishing e malware aprenderão com isso após algumas semanas. Até lá, para bloqueiá-lo, crie uma entrada de bloco na lista de permissões/blocos do locatário, se ainda não tiver sido feito |
| goodReclassifiedAsBulk                 | A Microsoft considera a mensagem relatada spam. Os filtros de spam e em massa aprenderão com isso após algumas semanas. Até lá, para bloqueiá-lo, crie uma entrada de bloco na lista de permissões/blocos do locatário, se ainda não tiver sido feito |
| goodReclassifiedAsGood                 | A Microsoft considera a mensagem relatada limpa. Se você não concordar com este veredicto, envie novamente o email. Até lá, para bloqueiá-lo, crie uma entrada de bloco na lista de permissões/blocos do locatário, se ainda não tiver sido feito |
| goodReclassifiedAsCannotMakeDecision   | A Microsoft não pode chegar a um veredicto no momento. Reenvie-o para obter um veredicto após a análise. Use a lista de permissões/bloqueios de locatário para bloqueiá-la imediatamente se ainda não tiver feito isso. |
| badReclassifiedAsGood                  | A Microsoft considera a mensagem relatada limpa. Emails existentes foram liberados. Os filtros de phishing e malware aprenderão com isso após algumas semanas. Até lá, para permitir, crie uma entrada de permissão na lista de permissões/bloqueios do locatário, se ainda não tiver sido feito |
| badReclassifiedAsBulk                  | A Microsoft considera a mensagem relatada spam. Os filtros de spam e em massa aprenderão com isso após algumas semanas. Até lá, para permitir, crie uma entrada de permissão na lista de permissões/bloqueios do locatário, se ainda não tiver sido feito |
| badReclassifiedAsBad                   | A Microsoft considera a mensagem relatada mal-intencionada. Se você não concordar com este veredicto, envie novamente o email. Até lá, para permitir, crie uma entrada de permissão na lista de permissões/bloqueios do locatário, se ainda não tiver sido feito |
| badReclassifiedAsCannotMakeDecision    | A Microsoft não pode chegar a um veredicto no momento. Reenvie-o para obter um veredicto após a análise. Use a lista de permissões/bloqueios de locatário para permitir imediatamente, caso ainda não tenha feito isso. |
| unknownFutureValue                     | Qualquer valor futuro que não esteja em uso agora.                     |


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.submissionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.submissionResult",
  "category": "String",
  "detail": "String",
  "userMailboxSetting": "String",
  "detectedUrls": [
    "String"
  ],
  "detectedFiles": [
    {
      "@odata.type": "microsoft.graph.security.submissionDetectedFile"
    }
  ]
}
```

