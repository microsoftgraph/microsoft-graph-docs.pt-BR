# <a name="compliancestate-enum-type"></a>tipo enumerado complianceState

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Estado de conformidade.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|unknown|0|Desconhecido.|
|em conformidade|1|Em conformidade.|
|sem conformidade|2|Dispositivo não está em conformidade e está bloqueado para recursos corporativos.|
|conflito|3|Conflito com outras regras.|
|erro|4|Erro|
|prazo de tolerância|254|Dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos|
|configManager|255|Gerenciado pelo Gerenciador de configuração|








