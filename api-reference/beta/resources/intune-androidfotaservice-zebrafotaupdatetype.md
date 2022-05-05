---
title: Tipo de enumeração zebraFotaUpdateType
description: Representa vários tipos de atualização para a implantação do Zebra FOTA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5bd17423e3a158a2010ae0afac18b56e406e1651
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213045"
---
# <a name="zebrafotaupdatetype-enum-type"></a>Tipo de enumeração zebraFotaUpdateType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa vários tipos de atualização para a implantação do Zebra FOTA.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Personalizado|0|Atualização personalizada em que o usuário seleciona BSP, versão do sistema operacional e número de patch específicos para atualizar.|
|Últimas|1|A atualização mais recente lançada se torna o sistema operacional de destino. A versão mais recente pode atualizar o dispositivo para uma nova versão do Android.|
|Automático|2|O dispositivo sempre procura o pacote mais recente disponível no repositório e tenta atualizar sempre que um novo pacote está disponível. Isso continuará até que o administrador cancele a atualização automática.|
|unknownFutureValue|99|Valor de enumeração futuro desconhecido.|




